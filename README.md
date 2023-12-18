# HM-CI-with-Jackknife-Bootstrap
We explore the use of jackknife and bootstrap methods as discussed in "Using resampling techniques to compute confidence intervals for the harmonic mean of rate-based performance metrics" [https://ieeexplore.ieee.org/abstract/document/5394469/?casa_token=qpyuFudV8W4AAAAA:M9qfunBLB-BcTaydzKOfdPSdGAmXG3sTcOtIPsdbTtc8178XkcIKjSOjz94qBSJ11WJY11KnsZM].
The .ipynb files contain the code and also the results of each cell.
Jackknife and Bootstrap  statistical resampling method is a way to determine the confidence interval for the harmonic mean of rate-based metrics like FLOPs, IPC, and so on. 
The ideal way to calculate the Confidence Interval for the Arithmetic mean doesn't yield the right answer for the Harmonic mean due to differences in the mathematical derivation. The paper mentioned above discusses the use of a non-parametric method for resampling to calculate the Confidence Interval (C.I.) of the Harmonic Mean. 

we perform random sampling on the given dataset, the IPC of the processor when executing a specific program, using the Jackknife and Bootstrap method. We are given a set of IPC measures with 13 samples in the set. We perform random sampling to calculate the harmonic mean of IPC values as the function of K. We perform random sampling with a bootstrap method for k times, and for each k we perform 20 iterations expecting to get a better outcome. We implemented a Python code for the confidence interval calculation and found that the 90% confidence interval using the Jackknife technique is (0.7332,0.9794), and 95% confidence interval using the Bootstrap method yields a confidence interval of a lot as seen in the chart below. Our work is based on the paper by Patil and Lilja mentioned in the reference section. Monte Carlo simulation is used by the authors in justifying the effectiveness of the jackknife and bootstrap method for calculating the confidence interval the of harmonic mean.
# Results
![image](https://github.com/Prithviraj97/HM-CI-with-Jackknife-Bootstrape/assets/60533093/7039802a-f11b-4f74-b4b4-42ddad6ae8cd)
![c2](https://github.com/Prithviraj97/HM-CI-with-Jackknife-Bootstrape/assets/60533093/861ae9f7-e140-417b-988e-bafa558a3caf)
![c1](https://github.com/Prithviraj97/HM-CI-with-Jackknife-Bootstrape/assets/60533093/f3c9eefd-7dba-4b86-9d69-fc708cbb2d65)
![c3](https://github.com/Prithviraj97/HM-CI-with-Jackknife-Bootstrape/assets/60533093/36125125-d3f2-4f88-bc1a-c57f061a3a02)
