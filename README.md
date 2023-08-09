Spam Filter Project
Overview
This project involved building a machine learning model to classify text messages as spam or ham (not spam). The CRISP-DM process was followed, including business understanding, data understanding, data preparation, modeling, evaluation, and deployment phases.

The goals were to:

Organize the project structure using Git and CRISP-DM
Analyze the provided dataset
Preprocess and vectorize the text data
Build classification models to identify spam messages
Evaluate models and perform error analysis
Choose the best performing model and package it for deployment
Data Understanding
The training dataset contained 5572 text messages labeled as either spam or ham. It was imbalanced, with only 13.4% spam messages and 86.6% ham.

The spam messages contained certain common words frequently like "free", "win", "prize", etc.

While the ham messages contained more normal vocabulary.

Modeling
Multiple classification models were trained and evaluated, including Logistic Regression, Naive Bayes, SVM, and Random Forest. The Multinomial Naive Bayes model performed the best with 99% accuracy.

Evaluation
The Multinomial Naive Bayes model achieved:

99% Accuracy
98% Precision
93% Recall
96% F1-Score
The confusion matrix shows the prediction breakdown:

Conclusion
The Multinomial Naive Bayes model was the best performer and was packaged and deployed for filtering new message data in production. The model achieved high accuracy, precision, recall and F1 score.

Future Work
Collect more training data over time to retrain model and improve performance
Address class imbalance with techniques like oversampling
Try deep learning approaches like RNNs or transformers
Local Setup
To run this project locally:

Clone the repo
Create conda environment from env.yaml
Activate environment and run Jupyter notebook

git clone [https://github.com/<repo>](https://github.com/seyedfarhadtorabi/spam_filter.git)
conda env create -f environment.yaml
conda activate <env>
jupyter notebook
