# Fake-News-Detection-Using-Machine-Learning

## **Project Overview**

### **What Am I Doing?**
This project focuses on building a machine learning model to classify news articles as either **True** or **Fake** using a binary classification approach. The project uses the **True vs Fake News Detection dataset** from Kaggle to train and evaluate the model.

### **How Am I Doing It?**
The project will follow a structured machine learning workflow, which includes:
1. **Data Preprocessing**: Cleaning and preparing the text data for training.
2. **Feature Extraction**: Converting the text into numerical vectors using techniques such as **TF-IDF** or **Word Embeddings**.
3. **Model Training**: Building and training machine learning models such as **Naive Bayes**, **Logistic Regression**, and **Neural Networks**.
4. **Model Evaluation**: Using test data to evaluate model performance based on accuracy, precision, recall, and F1-score.
5. **Model Improvement**: Iterating on model improvements by fine-tuning hyperparameters and exploring advanced techniques.

### **Why Am I Doing It?**
The rise of fake news has become a critical issue in today’s media landscape, with misinformation having potentially harmful consequences. By developing an automated system to classify news articles as **True** or **Fake**, this project aims to contribute to efforts to curb the spread of misinformation online.

---

## **Dataset Information**

### **Dataset Source**: [Kaggle True vs Fake News Detection Dataset](https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets/data)

### **Dataset Components**:
- **true.csv**: Contains news articles that are confirmed to be true.
- **fake.csv**: Contains news articles that are classified as fake.

Each file contains the following columns:
- **title**: The headline of the news article.
- **text**: The body text of the article.
- **label**: For labeling purposes, 1 represents **True** news and 0 represents **Fake** news (if this is not included in the dataset, we will label it manually).

### **Training and Testing Split**:
- **Training Data**: 80% of the dataset will be used for training the models.
- **Test Data**: 20% of the dataset will be set aside to evaluate model performance on unseen data.

---

## **Milestone Plan**

### **1. Data Preparation**
#### **Goal**:
Prepare the dataset for modeling by cleaning, preprocessing, and splitting it into training and testing sets.

#### **Steps**:
- [ ] **Load Data**:
   - Import both `true.csv` and `fake.csv` into a single DataFrame, labeling each article as either **True (1)** or **Fake (0)**.

- [ ] **Data Cleaning**:
   - Remove any duplicates or missing values.
   - Convert text to lowercase, remove punctuation, and clean up special characters.

- [ ] **Train-Test Split**:
   - Split the dataset into **80% training data** and **20% test data** for evaluation.

- [ ] **Exploratory Data Analysis (EDA)**:
   - Perform EDA to understand the distribution of true vs fake news, word counts, and any patterns in the dataset.

#### **Deliverables**:
- [ ] Cleaned and labeled dataset.
- [ ] Dataset split into training and test sets.
- [ ] Exploratory data analysis summary and visualizations.

---

### **2. Feature Extraction**
#### **Goal**:
Convert the text data into a numerical format that can be fed into machine learning models.

#### **Steps**:
- [ ] **TF-IDF Vectorization**:
   - Apply **TF-IDF** vectorization to convert both the headlines and body text into numerical features.
   - Ensure the vector size is consistent for both the true and fake news samples.

- [ ] **Word Embeddings (Optional)**:
   - Optionally, explore using **Word2Vec** or **GloVe** word embeddings for richer text representations.

- [ ] **Feature Selection**:
   - Explore feature importance to identify which words or phrases are most predictive of fake or true news.

#### **Deliverables**:
- [ ] TF-IDF vectors for the dataset.
- [ ] Optional word embeddings for deeper text representation.
- [ ] Analysis of important features for classification.

---

### **3. Model Selection and Implementation**
#### **Goal**:
Build and train machine learning models to classify news articles as true or fake.

#### **Methods**:
1. **Baseline Model (Naive Bayes)**:
   - [ ] Implement a **Naive Bayes classifier** as a baseline for the classification task.

2. **Logistic Regression**:
   - [ ] Train a **Logistic Regression model** as another baseline for comparison.
   - [ ] Tune hyperparameters such as regularization to improve performance.

3. **Neural Network (PyTorch)**:
   - [ ] Build and train a **simple neural network** using **PyTorch**.
   - [ ] Use multiple layers with **ReLU activation** and a **softmax output** for binary classification.

4. **Training**:
   - [ ] Train all models on the **80% training data**.
   - [ ] Evaluate the models using **cross-validation**.

5. **Evaluation**:
   - [ ] Evaluate the models on the **20% test data** using metrics like **accuracy, precision, recall, and F1-score**.

#### **Deliverables**:
- [ ] Trained Naive Bayes, Logistic Regression, and Neural Network models.
- [ ] Evaluation metrics for each model.
- [ ] Cross-validation results for each model.

---

### **4. Model Evaluation and Results**
#### **Goal**:
Analyze the performance of the models and compare their results.

#### **Steps**:
- [ ] **Confusion Matrix**:
   - Generate confusion matrices for each model to understand how well they classify true and fake news.

- [ ] **Model Comparison**:
   - Compare the models’ performance based on accuracy, precision, recall, and F1-score.
   - Analyze the trade-offs between simple models (Naive Bayes, Logistic Regression) and more complex models (Neural Networks).

- [ ] **Strongest Features**:
   - Identify the most predictive words or phrases from the TF-IDF features for both true and fake news.

#### **Deliverables**:
- [ ] Confusion matrices for all models.
- [ ] Model comparison based on evaluation metrics.
- [ ] Analysis of key features that predict fake news.

---

### **5. Strategy for Improvement**
#### **Goal**:
Develop strategies to further improve the model’s performance and robustness.

#### **Steps**:
1. **Hyperparameter Tuning**:
   - Fine-tune the hyperparameters of all models (e.g., learning rate, regularization, number of hidden layers for neural networks).

2. **Ensemble Methods**:
   - Explore combining models using ensemble methods such as **Voting Classifier** or **Stacking** to improve accuracy.

3. **Advanced Neural Networks**:
   - Experiment with deeper neural network architectures or **Convolutional Neural Networks (CNNs)** for better text feature extraction.

4. **Data Augmentation**:
   - Explore techniques like **synthetic data generation** to increase the diversity of training data.

#### **Deliverables**:
- [ ] Plan for hyperparameter tuning and model improvements.
- [ ] Ensemble model implementation (optional).
- [ ] Suggested improvements in model architecture for advanced models.

---

## **Justification**
### **Why Am I Using These Methods?**
- **Naive Bayes**: A fast and interpretable baseline for text classification.
- **Logistic Regression**: A simple but powerful linear classifier for binary classification.
- **Neural Networks (PyTorch)**: More complex models capable of capturing deeper patterns in text data, especially useful for larger datasets.

---

## **Final Deliverables**
### **Goal**:
Summarize the final deliverables for the project.

1. **Cleaned Dataset**: Processed and labeled dataset with true and fake news articles.
2. **Model Implementations**:
   - Trained Naive Bayes, Logistic Regression, and Neural Network models.
3. **Evaluation Results**:
   - Confusion matrices, accuracy, precision, recall, and F1-score for all models.
4. **Documentation**:
   - Complete project documentation explaining methods, results, and suggestions for future work.
