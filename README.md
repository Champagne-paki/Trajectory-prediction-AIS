# Trajectory-prediction-AIS
This project evaluates the performance of 1D-CNN and DNN models in trajectory prediction of vessels in the East Asian region

Model Performance Comparison: CNN vs DNN
1. Validation Set (Training Feedback Performance)
Metric	CNN	DNN	Better Model
Val MAE	0.01325	0.01334	 CNN (slightly)
Val MSE	0.000277	0.000320	 CNN

 CNN shows slightly better performance on the validation set, suggesting it learned patterns more accurately during training.

2. Test Set (Generalization Performance)
Metric	CNN	DNN	Better Model
Test ADE	0.01980	0.01931	 DNN
Test FDE	0.02487	0.02086	 DNN
Test NL-ADE	0.02541	0.02775	 CNN

 DNN outperforms CNN on test ADE and FDE, showing better average and final displacement predictions.
 CNN performs better on NL-ADE, indicating superior handling of non-linear trajectory changes (e.g., sharp turns).

