## 1. Overview

Walmart Recruiting: Trip Type Classification
- https://www.kaggle.com/c/walmart-recruiting-trip-type-classification

### Team - 10 to 10
- Kim DH
- Jang HW
- Kim HS

### Objective
To classify customer trips using only a transactional dataset of the items

## 2. Dataset Description
- Train : 640,754 rows × 7 columns
- Test : 653,646 rows × 6 columns

Features|Types of Variable|Feature Description|Unique Value
--------|------------|------------|----------
TripType|Categorical|a categorical id representing the type of shopping trip the customer made|38
VisitNumber|Categorical|an id corresponding to a single trip by a single customer|95674
DepartmentDescription|Categorical|a high-level description of the item's department|68
FinelineNumber|Categorical|a more refined category for each of the products, created by Walmart|5196
Upc|Categorical|the UPC number of the product purchased|97715
Weekday|Categorical|the weekday of the trip|7
Scancount|Numerical|the number of the given item that was purchased|

## 3. Evaluation
- the multi-class logarithmic loss

## 4. Modeling
- train data

Model|Accuracy|log loss
-----|--------|--------
logistic|0.723|0.964
Random Forest|0.534|1.816
**light GBM**|**0.888**|**0.716**

## 5. Result
- Kaggle score : 0.80596
