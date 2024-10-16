# Causal Feature Selection via Adaptive Scaling Down (ASD) $G^2$-Test
This project implements an ASD $G^2$-test for causal feature selection algorithms. Compared to classical $G^2$-test, the ASD $G^2$-test significantly enhances the accuracy and robustness of feature selection.

## Project Structure

- `benchmark_BN`: Contains code for running on benchmark datasets.
- `RealWorld_datasets`: Contains code for running on real-world datasets.

## Instructions for Use

### Benchmark Datasets

To run the benchmark_BN data, go to the benchmark_BN folder and run main.py

First, enter the name of the benchmark dataset you wish to run. The available datasets are: alarm, barley, child, insurance, munin1, pigs.

Then, choose whether to use the original datasets by selecting yes or no.

if yes：

    Choose the sample size: 1000, 2000, 5000.
    
    Select the MB discovery algorithm: "IAMB", "MMMB", "FBEDk", "HITON-MB", "STMB", "MBOR", "BAMB".
    
    Select the CI test: Choose 1-4: classical G2test=1,ASD G2test=2,chi-squared test=3,fisher_z test=4.

    Run to generate results.
    
if no：

    Enter the sample size to generate new data.
    
    Select the MB discovery algorithm: "IAMB", "MMMB", "FBEDk", "HITON-MB", "STMB", "MBOR", "BAMB".
    
    Select the CI test: Choose 1-4: classical G2test=1,ASD G2test=2,chi-squared test=3,fisher_z test=4.

    Run to generate results.

### Real-World Datasets

To run the RealWorld_datasets, go to the RealWorld_datasets folder and run main.py:

Enter the name of the real-world dataset you wish to run. The available datasets are: "breast-cancer", "chess", "cmc", "congress", "mushroom", "splice".

Select the MB discovery algorithm: "IAMB", "MMMB", "FBEDk", "HITON-MB", "STMB", "MBOR", "BAMB".

Select the CI test: Choose 1-4: classical G2test=1,ASD G2test=2,chi-squared test=3,fisher_z test=4.

Run to generate results.

## Dependencies

Make sure you have installed the following Python libraries:

- `numpy`
- `pandas`
- `scikit-learn`
- Additional dependencies might be required. Please check the code for further dependencies.


