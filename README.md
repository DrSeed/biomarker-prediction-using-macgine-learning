In this study, I explored the utility of 48 candidate Differentially Expressed Genes (DEGs) in constructing a diagnostic classification model for Pulmonary Arterial Hypertension (PAH). I employed seven different machine learning algorithms to evaluate their performance in accurately diagnosing PAH. The algorithms' effectiveness was assessed through a rigorous validation process utilizing five repeated five-fold cross-validation techniques.

Model Performance and Selection
This analysis revealed that models based on Gradient Boosting Decision Tree (GBDT) algorithms delivered superior performance. Notably, the GBDT models achieved a remarkable mean Area Under the Curve (AUC) value of 1 and an accuracy rate of 93%, outshining the other models we tested. This led us to select GBDT for our final diagnostic classification model for PAH.

While Extreme Gradient Boosting (XGBoost) is renowned for its efficacy in handling high-dimensional datasets, it did not yield superior results in our study, possibly due to the limited size of our dataset.

Model Evaluation and Biomarker Identification
The evaluation of model performance was visually represented through Receiver Operating Characteristic (ROC) curves for each fold in the testing set. An observation from this analysis was the rigid appearance of the curves, which we attributed to the binary nature of the output probabilities ([0, 1] or [1, 0]) inherent in tree-based models. This characteristic arises because the probabilities are directly linked to the class distribution of samples within a leaf node, which, in fully grown trees, tends to be homogenous.

Despite these observations, our decision on the optimal model was informed by both the AUC and accuracy metrics, ensuring a comprehensive assessment of model performance.


Conclusion
This exploration into machine learning-based diagnostic models for PAH highlights the potential of GBDT algorithms, backed by a select set of biomarkers, in accurately diagnosing the condition. The insights gleaned from this study could pave the way for more refined diagnostic tools for PAH, subject to validation in larger datasets.
