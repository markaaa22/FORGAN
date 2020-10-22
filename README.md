# ForGAN
Pytorch implementation of "[Probabilistic Forecasting of Sensory Data with Generative Adversarial Networks - ForGAN](https://ieeexplore.ieee.org/abstract/document/8717640)"

ForGAN is one step ahead probabilistic forecasting which utilizes the power of the conditional generative adversarial network to learn the data generating distribution and compute probabilistic forecasts from it.

We tested ForGAN against two publicly available datasets, namely Mackey-Glass dataset and Internet traffic dataset (A5M), and a new dataset, Lorenz dataset, where the impressive performance of ForGAN demonstrates its high capability in forecasting future values.

## Lorenz dataset
The Lorenz dataset is generated using the Lorenz system which contains multiple time window clusters. Each cluster consists of similar and complex time series where the value of the next step follows a probability distribution. You can find more information in the paper.

## Mackey-Glass dataset
The time delay differential equation suggested by Mackey and Glass has been used widely as a standard benchmark model to generate chaotic time-series for the forecasting task.

## Internet Traffic dataset (A5M)
Internet Traffic dataset belongs to a private ISP with centers in eleven European cities (which is commonly known as A5M). It contains data corresponding to a transatlantic link and was collected in 2005 from 06:57 on 7th of June to 11:17 on 29th of July.

## Metric and results
With code provided here, you should be able to reproduce values reported in the paper. Beside RMSE, MAE, MAPE, and KLD, this code also reports  "continuous ranked probability score (CRPS)". CRPS is a measure of performance for probabilistic forecasts of a scalar observation. CRPS is comparable to the MAE of the deterministic model. As a result, the direct comparison of the probabilistic and non-probabilistic models becomes possible.

# Environment
Python = 3.6.8
Pytorch = 1.0.1

# Acknowledgement
This work has been conducted in FLaP lab. FLaP is a joint lab between IAV GmbH and DFKI GmbH. IAV is a leading engineering company in the automotive industry, designing products for powertrain, electronics, and vehicle development. DFKI is the german research center for artificial intelligence which is one of the leading AI research centers in Germany.