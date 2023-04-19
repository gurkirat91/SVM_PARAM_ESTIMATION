# Parameter-Optimisation-SVM


**Dataset Used:** [Wine Quality Dataset (White-Wine)](https://archive.ics.uci.edu/ml/datasets/wine+quality)

**Data Set Information**:

The two datasets are related to red and white variants of the Portuguese "Vinho Verde" wine. For more details, consult: [Web Link] or the reference [Cortez et al., 2009]. Due to privacy and logistic issues, only physicochemical (inputs) and sensory (the output) variables are available (e.g. there is no data about grape types, wine brand, wine selling price, etc.).

These datasets can be viewed as classification or regression tasks. The classes are ordered and not balanced (e.g. there are many more normal wines than excellent or poor ones). Outlier detection algorithms could be used to detect the few excellent or poor wines. Also, we are not sure if all input variables are relevant. So it could be interesting to test feature selection methods.


**Attribute Information**:

For more information, read [Cortez et al., 2009]. 
Input variables (based on physicochemical tests): 
1 - fixed acidity 
2 - volatile acidity 
3 - citric acid 
4 - residual sugar 
5 - chlorides 
6 - free sulfur dioxide 
7 - total sulfur dioxide 
8 - density 
9 - pH 
10 - sulphates 
11 - alcohol 
Output variable (based on sensory data): 
12 - quality (score between 0 and 10)


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
