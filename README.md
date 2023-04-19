# Parameter-Optimisation-SVM


**Dataset Used:** [Wine Quality Dataset (White-Wine)](https://archive.ics.uci.edu/ml/datasets/wine+quality)

| Number of Instances:  | 5898  |
|-----------------------|--------|
| Number of Attributes: | 12     |

---

**Parameter Grid Used**
---
|Hyperparameter         |Values                |
|-----------------------|----------------------|
| kernel                | 'linear', 'poly', 'rbf', 'sigmoid' |
| C                     | [0.1, 1, 10]    |
| gamma                 | [0.1, 1, 10]   |

---
 
 | Sample Number | Best Accuracy | Kernel | C  | gamma |
|----------|---------------|--------|-----|-------|
| 1        | 0.4533       | rbf    | 1.000 | 0.1   |
| 2        | 0.4633        |  poly    | 1.000 | 1   |
| 3        | 0.4700        | rbf    | 1.000 | 1   |
| 4        | 0.4833        | rbf    | 1.000 | 0.1   |
| 5        | 0.4933        | rbf    | 10.000 | 1  |
| 6        | 0.4967        | rbf    | 1.000 | 10  |
| 7        | 0.5200        | rbf    | 10.000 | 1   |
| 8        | 0.4733        | rbf    | 10.000 | 1   |
| 9        | 0.4967        | rbf    | 1.000 | 1   |
| 10       | 0.4933        | rbf    | 1.000 | 0.1 |

---

**Sample 7 gives the Best SVM accuracy with params: rbf,10.000,1 for Kernel,C and Gamma respectively**

---

Graph of Accuracy per 1000 iterations for Sample 7:

![alt text](https://github.com/gurkirat91/SVM_PARAM_ESTIMATION/blob/main/Screenshot%202023-04-20%20at%201.04.10%20AM.png)
