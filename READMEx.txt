Data
-recipe_train.csv
-recipe_test.csv
-recipe_text_features_countvec
	-train_ingr_vec.npz
	-train_name_vec.npz
	-train_steps_vec.npz
	(for kaggle)
	-test_ingr_vec.npz
	-test_name_vec.npz
	-test_steps_vec.npz
-recipe_text_features_doc2vec100
	-train_ingr_doc2vec100.csv
	-train_name_doc2vec100.csv
	-train_steps_doc2vec100.csv
	(for kaggle)
	-test_ingr_doc2vec100.csv
	-test_name_doc2vec100.csv
	-test_steps_doc2vec100.csv

Notebook
-logist_svm.ipynb : 
contains logistic regression and svm model. 
Feature selection is also done here.
-xgboost_stack.ipynb :
contains xgboost and stacking model.
predicting test data for kaggle is done here.

Steps
Run cells in logist_svm.ipynb in order.
This produces a csv file containing logistic regression
and svm predictions for stacking.
Run cells in xgboost_stack.ipynb in order.
To reproduce results of xgboost, manually change learning_rate.
