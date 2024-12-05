Here’s a plain list of common hyperparameters used in grid search for popular machine learning models:

---

### **Linear Models**
#### Logistic Regression / Linear Regression
- `penalty`: `l1`, `l2`, `elasticnet`, `none`
- `C`: `[0.01, 0.1, 1, 10, 100]`
- `solver`: `newton-cg`, `lbfgs`, `liblinear`, `sag`, `saga`
- `max_iter`: `[100, 200, 500]`
- `l1_ratio`: Only for `penalty='elasticnet'`

---

### **Support Vector Machines**
#### SVC / SVR
- `C`: `[0.1, 1, 10, 100]`
- `kernel`: `linear`, `poly`, `rbf`, `sigmoid`
- `degree`: `[2, 3, 4]` (for `kernel='poly'`)
- `gamma`: `scale`, `auto`, or `[0.001, 0.01, 0.1, 1]`
- `epsilon`: For SVR

---

### **Decision Trees**
#### DecisionTreeClassifier / DecisionTreeRegressor
- `criterion`: `gini`, `entropy`, `squared_error`, `friedman_mse`, `absolute_error`
- `max_depth`: `[5, 10, 15, None]`
- `min_samples_split`: `[2, 5, 10]`
- `min_samples_leaf`: `[1, 2, 4]`
- `max_features`: `auto`, `sqrt`, `log2`, or integers

---

### **Random Forest**
#### RandomForestClassifier / RandomForestRegressor
- `n_estimators`: `[10, 50, 100, 200]`
- `criterion`: Same as Decision Trees
- `max_depth`: Same as Decision Trees
- `min_samples_split`: Same as Decision Trees
- `min_samples_leaf`: Same as Decision Trees
- `max_features`: Same as Decision Trees
- `bootstrap`: `True`, `False`

---

### **Gradient Boosting**
#### GradientBoostingClassifier / GradientBoostingRegressor
- `n_estimators`: `[100, 200, 300]`
- `learning_rate`: `[0.01, 0.1, 0.2, 0.3]`
- `max_depth`: `[3, 5, 7]`
- `min_samples_split`: Same as Decision Trees
- `min_samples_leaf`: Same as Decision Trees
- `subsample`: `[0.6, 0.8, 1.0]`
- `max_features`: Same as Decision Trees

---

### **XGBoost**
#### XGBClassifier / XGBRegressor
- `n_estimators`: `[50, 100, 200]`
- `learning_rate`: `[0.01, 0.1, 0.2, 0.3]`
- `max_depth`: `[3, 5, 7, 10]`
- `min_child_weight`: `[1, 3, 5]`
- `subsample`: `[0.6, 0.8, 1.0]`
- `colsample_bytree`: `[0.6, 0.8, 1.0]`
- `gamma`: `[0, 1, 5]`
- `lambda`: `[0, 1, 5]`
- `alpha`: `[0, 1, 5]`

---

### **k-Nearest Neighbors**
#### KNeighborsClassifier / KNeighborsRegressor
- `n_neighbors`: `[3, 5, 7, 10]`
- `weights`: `uniform`, `distance`
- `metric`: `euclidean`, `manhattan`, `minkowski`

---

### **Neural Networks**
#### MLPClassifier / MLPRegressor
- `hidden_layer_sizes`: `[(50,), (100,), (50, 50)]`
- `activation`: `identity`, `logistic`, `tanh`, `relu`
- `solver`: `lbfgs`, `sgd`, `adam`
- `alpha`: `[0.0001, 0.001, 0.01]`
- `learning_rate`: `constant`, `invscaling`, `adaptive`
- `max_iter`: `[200, 500, 1000]`

---

### **Naive Bayes**
#### GaussianNB / MultinomialNB
- `var_smoothing`: `[1e-9, 1e-8, 1e-7]` (GaussianNB)
- `alpha`: `[0.1, 1.0, 10.0]` (MultinomialNB)

--- 



