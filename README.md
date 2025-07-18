#  Vessel Trajectory Prediction with AIS Data: CNN vs DNN Comparison

This project compares the performance of a **1D CNN model** and a **Deep Neural Network (DNN)** for vessel trajectory prediction using AIS (Automatic Identification System) data in the East Asian Region.

---

##  Model Performance Comparison

###  1. Validation Set (Training Feedback Performance)

| Metric        | CNN        | DNN        | Better Model |
|---------------|------------|------------|---------------|
| **Val MAE**   | 0.01325    | 0.01334    |  CNN |
| **Val MSE**   | 0.000277   | 0.000320   |  CNN |

> **CNN** shows slightly better accuracy during validation, indicating better fit during training.

---

### 📦 2. Test Set (Generalization Performance)

| Metric        | CNN         | DNN         | Better Model |
|---------------|-------------|-------------|---------------|
| **Test ADE**  | 0.01980     | 0.01931     |  DNN |
| **Test FDE**  | 0.02487     | 0.02086     |  DNN |
| **Test NL-ADE**| 0.02541    | 0.02775     |  CNN |

> **DNN** shows superior generalization on unseen data in both average and final displacement.  
> **CNN** performs better in handling non-linear trajectories, useful for erratic routes.

---

## 📈 Map of Trajectories

<img width="950" height="787" alt="image" src="https://github.com/user-attachments/assets/f47cdb36-d020-42bf-8b0a-6f7eb43a8903" />

<img width="841" height="624" alt="image" src="https://github.com/user-attachments/assets/819de202-950d-42ff-9882-38a8fe7ffdf3" />



---

