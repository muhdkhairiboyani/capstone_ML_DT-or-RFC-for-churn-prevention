##### Capstone: Machine Learning with Python
---
---
# CHOOSING BETWEEN DECISION TREE & RANDOM FOREST FOR CUSTOMER CHURN

Purpose:
The purpose of this project is to look at two machine learning models and find out the following:

Which ML model has better accuracy score to predict churn.
Are there similarities and differences between them?
Dataset:
The dataset used in this project is a set of data from a bank in the US, and they are experiencing customer churn - Kaggle.

Enquirer:
The boss of ACDC Pte Ltd wants to know which machine learning model - Decision Tree OR Random Forest Classifier - will be the better model to predict customer churn.

**Data source:**
https://www.kaggle.com/datasets/shantanudhakadd/bank-customer-churn-prediction

### 02 EDA & DATA PRE-PROCESSING
List of libraries \
![](13-import-library.png)

Gathering insights of data \
![](14-data-overview.png)

The data has NO missing values and also NO duplicates.
![](16-missing-values.png)
![](17-no-duplicates.png)

Three columns are Drop.
![](18-drop-3-columns.png)

Heatmap (Seaborn) is generated to identify any coorelations between classes.
![](01-Heatmap.jpg)

### 03 Visualization of dataset
In general, there are more Males than Females in the dataset. However, more Females churn than Male.
![](02-No-of-Females-and-Males.jpg)
![](03-Gender-Exited.png)

When we look at churn by Geography, the bank has more customer from France. But churn customers from France and Germany are almost equal.
![](04-Geography-Exited.png)

Other visualization based on this dataset:
![](05-3x3-Subplot.jpg)

### 04 PREPARING DATA for building Machine Learning Models
![](15-preparing-data.png)

Using a Scatter Matrix, we can observe some areas that might contribute to customer churn - Age, Num of products, credit score and tenure.
![](06-Scatter-Matrix.jpg)

### 05 Build Machine Learning Model
Train and Test:
A Train size of 75 and Test size of 25 are set for training and testing ML models: Random Forest and Decision Tree.

#### RANDOM FOREST
Random Forest Accuracy Test Score:
![](19-rfc-accuracy-test.png)

Random Forest Confusion Matrix:
![](07-CM-Random-Forest.jpg)

Feature_Importance bar chart highlights 5 classes that need attention in order to predict and prevent churn.
![](08-Feature-Importance.jpg)

Visual of Random Forest
![](09-Random-Forest-Tree.jpg)

#### DECISION TREE
Decision Tree Accuracy Test Score:
![](20-dt-accuracy-test.png)

Decision Tree Confusion Matrix:
![](10-CM-Decision-Tree.jpg)

Visual of Decistion Tree
![](11-Decision-Tree.jpg)

### 07 Receiver Operator Characteristic (ROC) Curve and Area under the Curve (AuC)
Plotting the ROC curve and obtaining the AuC score proves to be the deciding factor as to which machine learning model fare better than the other.
![](12-ROC-Curve.jpg)

### 08 CHOOSING between Decision Tree and Random Forest:

**Which ML model has better accuracy score to predict churn.**
The ROC curve and the AuC score shows that Random Forest is more robust in making complex predictions and it has better accuracy.

**Are there similarities and differences between them.**
**DECISION MAKING**
**Decision tree** combines some decisions.  
**Random forest** combines several **decision trees**. 

**PROCESSING**
**Decision tree** is fast and operates easily on large data sets, especially the linear one.
**Random forest** is a long process, yet slow. Its model needs rigorous training.

**ACCURACY**
**Decision tree** accuracy can vary.
**Random forest** is highly accurate.

---

#### Contact me
- LinkedIn: [Muhammad Khairi](www.linkedin.com/in/muhammd-khairi-boyani-10694061)
- Instagram: [mikistudio21](https://www.instagram.com/mikistudio21/)

---
#### Platforms:
- Python
- Markdown: [dillinger](https://dillinger.io)

---


