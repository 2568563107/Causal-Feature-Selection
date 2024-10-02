# Causal Feature Selection via Adaptive Scaling Method (ASD) $G^2$-Test
本项目实现了一种改进的 $G^2$-test，用于因果特征选择。我们的方法通过IDOF和ASM提升了特征选择的准确性和效率。该方法适用于离散数据集。

## 项目结构

- `benchmark_BN`: 包含用于基准数据集的代码。
- `RealWorld_datasets`: 包含用于真实世界数据集的代码。

## 使用说明

### 基准数据集

要运行benchmark_BN数据，请在运行benchmark_BN文件夹中的main.py

此时请先输入你想运行的benchmark_BN名称，分别有alarm，barley，child，insurance，munin1，pigs

然后再选择是否使用original datasets，请选择yes，no

if yes：

    如果选择original datasets，请选择样本量1000，2000，5000
    
    选择MB发现算法，"IAMB", "MMMB", "FBEDk", "HITON-MB", "STMB", "MBOR", "BAMB"
    
    选择CI test，选择1-5，G2test=1,G2test_IDOF=2,G2test_IDOF_ASM=3,chi-squared test=4,fisher_z test=5

    运行产生结果
    
if no：

    选择样本量，生成新数据
    
    选择MB发现算法，"IAMB", "MMMB", "FBEDk", "HITON-MB", "STMB", "MBOR", "BAMB"
    
    选择CI test，选择1-5，G2test=1,G2test_IDOF=2,G2test_IDOF_ASM=3,chi-squared test=4,fisher_z test=5

    运行产生结果

### 真实世界数据集

要运行RealWorld_datasets,请在运行RealWorld_datasets文件夹中的main.py

此时请先输入你想运行的RealWorld_datasets，分别有"breast-cancer", "chess", "cmc", "congress", "mushroom", "splice"

然后选择MB发现算法，"IAMB", "MMMB", "FBEDk", "HITON-MB", "STMB", "MBOR", "BAMB"

选择CI test，选择1-5，G2test=1,G2test_IDOF=2,G2test_IDOF_ASM=3,chi-squared test=4,fisher_z test=5

运行产生结果

## 依赖

请确保你已经安装了以下 Python 库：

- `numpy`
- `pandas`
- `scikit-learn`
- 其他可能的依赖（请在代码中检查）


