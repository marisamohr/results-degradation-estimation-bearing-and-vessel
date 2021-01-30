# results-degradation-estimation-bearing-and-vessel

This repository contains the results of 104 experiments to estimate the degradation process for two different case studies each, one from manufacturing and one from dry-bulk shipping.

# Datasets
### Manufacturing
The data set used for the case study is the well-known bearing data set provided by FEMTO-ST institute within PRONOSTIA, an experimental platform dedicated to the testing and validation of bearing failure detection, diagnostic, and prognostic approaches.
The FEMTO bearing data set contains run-to-failure tests of 17 bearings, 6 for training and 11 for testing that can be found here: https://github.com/wkzs111/phm-ieee-2012-data-challenge-dataset. 


### Dry-Bulk-Shipping
The second data set consists of sensor data for 15 vessels, 12 for training and 3 for testing, with data ranging from beginning of 2016 to end of 2020. The data set is provided by an anonymous shipping company. 

# Notations for Experiments
We choose <img src="https://render.githubusercontent.com/render/math?math=Z_{i,j}">  to be an experiment, where <img src="https://render.githubusercontent.com/render/math?math=$Z\in\{A,\dots,M\}$"> denotes a combination of preprocessing steps listed in the table below, <img src="https://render.githubusercontent.com/render/math?math=$i\in\{\mathrm{true,false}\}$"> denotes if an health stage classifier is used, and <img src="https://render.githubusercontent.com/render/math?math=$j\in\{\text{MLR, GPR, ANN, SVR}\}$"> denotes the selected regression model for prediction, where <img src="https://render.githubusercontent.com/render/math?math=\text{MLR}$"> denotes Multiple Linear Regression, <img src="https://render.githubusercontent.com/render/math?math=\text{GPR}$"> denotes Gaussian Process Regression, <img src="https://render.githubusercontent.com/render/math?math=\text{ANN}$"> denotes Artificial Neural Network and <img src="https://render.githubusercontent.com/render/math?math=\text{SVR}$"> denotes Support Vector Machine.


<img width="442" alt="Bildschirmfoto 2021-01-29 um 11 53 38" src="https://user-images.githubusercontent.com/35696618/106266420-b0d69980-6228-11eb-9a6f-d4917cff2610.png">


For example, the notation <img src="https://render.githubusercontent.com/render/math?math=$E_{\mathrm{true},\mathrm{ANN}}$ "> represents the application of health stage classifier, followed by frequency analysis and statistical feature extraction, with a final regression of degradation using ANN. 



