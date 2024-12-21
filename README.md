# Multiclass_classification

This repository implements a multi-label classification pipeline for predicting Level 1 factors (e.g., Accessibility, Fragrance, Brand Value) from product reviews in the body wash domain.

Key Features

	1.	Data Processing:
	•	Group reviews by “Core Item” and convert Level 1 Factors into binary labels using MultiLabelBinarizer.
	2.	Exploratory Data Analysis:
	•	Visualize the distribution and proportions of Level 1 Factors using bar plots and pie charts.
	3.	Dataset Preparation:
	•	Split data into train and test sets.
	•	Tokenize text using BertTokenizer for sequence input.
	4.	Custom Dataset Class:
	•	Encodes inputs and labels into PyTorch tensors for model training.
	5.	Model Training:
	•	Fine-tune a BertForSequenceClassification model for multi-label classification.
	•	Utilize the Trainer API from Hugging Face for training and evaluation.
	6.	Evaluation:
	•	Compute predictions with a threshold of 0.5 using sigmoid activation.
	•	Generate classification metrics such as precision, recall, and F1-score.
	7.	Inference on Test Data:
	•	Predict labels for new reviews and save the results in an Excel file (predicted_labels.xlsx).
Technologies Used

	•	Model: BERT-base-uncased
	•	Framework: Hugging Face Transformers
	•	Visualization: Matplotlib, Seaborn
	•	Evaluation: Scikit-learn

Results

	•	Classification metrics (precision, recall, F1-score) are printed for validation data.
	•	Predicted labels for each review are available for further analysis.
