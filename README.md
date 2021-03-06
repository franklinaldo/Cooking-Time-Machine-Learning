# Cooking-Time-Machine-Learning

### Folders/files structure for training/test datasets

```
├── logist_svm.ipynb
├── xgboost_stack.ipynb
...
├── recipe_train.csv
├── recipe_test.csv
|
├── recipe_text_features_countvec
|   └── train_ingr_vec.npz
|   └── train_name_vec.npz
|    └── train_steps_vec.npz
|    (for kaggle)
|    └── test_ingr_vec.npz
|    └── test_name_vec.npz
|   └── test_steps_vec.npz
├── recipe_text_features_doc2vec100
    └── train_ingr_doc2vec100.csv
    └── train_name_doc2vec100.csv
    └── train_steps_doc2vec100.csv
    (for kaggle)
    └── test_ingr_doc2vec100.csv
    └── test_name_doc2vec100.csv
    └── test_steps_doc2vec100.csv
...
```

### Notebook
- ``` logist_svm.ipynb``` : 
contains logistic regression and svm model. 
Feature selection is also done here.
- ```xgboost_stack.ipynb``` :
contains xgboost and stacking model.
predicting test data for kaggle is done here.

### How to run :
1. Since the datasets are too big, you can download it from https://drive.google.com/drive/folders/1aT1O24Aw_fP5sPvSDFaUlsJ04k6volsv?usp=sharing. Place the datasets at the root level as shown in folder structure above.
2. Run cells in ``` logist_svm.ipynb ``` in order.
This produces a csv file containing logistic regression
and svm predictions for stacking.
3. Run cells in ``` xgboost_stack.ipynb ``` in order.
4. To reproduce results of xgboost, manually change learning_rate.

### Results
- prediction_xgboost_train_1_eta_0.2.csv
- pred_chi_750_svm_linear.csv
- pred kbest 750 chi2.csv
- stacking_predict.csv


<br>
Made by Franklin Darmansa and Nathen Kurniasurja