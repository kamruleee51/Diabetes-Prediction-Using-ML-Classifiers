# Diabetes Prediction Using Ensembling of Different Machine Learning Classifiers
Diabetes is a kind of metabolic diseases which forms by lack of insulin due to malfunctioning of pancreas. Diabetes can push a person into pathological destruction of pancreatic beta cells, coma, cardiovascular dysfunction, renal and retinal failure, joint failure, sexual dysfunction, pathogenic effects on immunity, weight loss, and peripheral vascular diseases. So, for the early detection of diabetes, a  robust  framework  was proposed where outlier rejection, filling the missing values, data standardization, K-fold validation, and different Machine Learning (ML) classifiers (k-NN, decision trees (DT), random forest (RF), adaBoost (AB), naive bayes (NB), and XGBoost (XB)) were used. To improve the result, weighted ensembling of different ML models also proposed here. The corresponding Area Under ROC Curve (AUC) of ML model as the performance metric estimated these weights. Using grid search technique, the AUC is then maximized during hyper-parameter tuning. All experiments were conducted under the same experimental conditions on publicly available Pima Indian population near Phoenix, Arizona of 768 female diabetic patients where there are 268 diabetic patients (positive) and 500 non-diabetic patients (negative) with eight different attributes. The proposed framework is shown in figure below.

![ProposedPipeline](https://user-images.githubusercontent.com/32570071/74607847-81597a80-5106-11ea-87f1-95e6adf69170.png)

After having Pima Dataset, we preprocessed the data like outlier rejection, filling missing values, data standardization, and dimensionality reduction of the attribute. After preprocessing, 5-fold Cross Validation technique is used for model selection and error estimation of classifiers. In our proposal, 4 folds and grid search algorithm were used to train and fine-tune the hyper-parameters in the inner loop whereas remaining fold is used for testing the model. After these processing, k-NN, DT, AB, RF, NB, and XB were implemented. Again, the ensembling of the ML model using a group of classifiers is used to improve the precision of the prediction. 

From all the models in the experiment, XGBoost performed better with sensitivity, specificity, false omission rate, diagnostic odds ratio, and AUC as: 0.768, 0.943, 0.100, 71.369, and 0.946 respectively. The proposed ensembling model outperforms XGBoost and state of the art results by 0.40 % and 2.00 % respectively in AUC. 

The more details of the proposed framework are coming soon- <br>

#### Written by-  <br>
Md. Kamrul Hasan <br> 
Erasmus Scholar on Medical Imaging and Application (MAIA) [2017-2019] [http://maiamaster.udg.edu/] <br> 
Assistant Professor <br>
Department of EEE, KUET, Khulna-9203, Bangladesh <br>
For more details write me at kamruleeekuet@gmail.com <br>
