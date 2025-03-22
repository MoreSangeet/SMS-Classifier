# Spam Message Classification

---

## Overview
This project is aimed at building a spam message classifier using machine learning. The goal is to classify messages as either "ham" (non-spam) or "spam" (unwanted messages). The classification model is built using various machine learning algorithms and natural language processing techniques.

## Table of Contents
1. [Project Description](#project-description)
2. [Technologies Used](#technologies-used)
3. [Dataset](#dataset)
4. [Steps Involved](#steps-involved)
5. [Model Evaluation](#model-evaluation)
6. [How to Run](#how-to-run)

## Project Description
This project is a spam message classification system. Using a dataset of labeled messages, we build a machine learning model to identify whether a message is spam or ham. Various preprocessing techniques like tokenization, stopword removal, and stemming are applied to prepare the text for machine learning models.

## Technologies Used
- **Python**: Programming language used for this project.
- **Pandas**: For data manipulation and analysis.
- **Numpy**: For numerical computations.
- **Sklearn**: For machine learning models and preprocessing.
- **Matplotlib & Seaborn**: For data visualization.
- **NLTK**: For natural language processing tasks like tokenization and stopword removal.
- **WordCloud**: To generate word clouds for data visualization.

## Dataset
The dataset used in this project is called **spam.csv**, which contains text messages and their respective labels (spam or ham).

The dataset has the following columns:
- `target`: 1 for spam, 0 for ham.
- `text`: The content of the message.

### Dataset Sample:
Here is a preview of a few rows from the dataset:

| Label | Message                                                                                 |
|-------|-----------------------------------------------------------------------------------------|
| ham   | Go until jurong point, crazy.. Available only in bugis n great world la e buffet...     |
| ham   | Ok lar... Joking wif u oni...                                                           |
| spam  | Free entry in 2 a wkly comp to win FA Cup final tkts 21st May 2005. Text FA to 87121... |
| ham   | U dun say so early hor... U c already then say...                                       |
| ham   | Nah I don't think he goes to usf, he lives around here though                           |
| spam  | FreeMsg Hey there darling it's been 3 week's now and no word back! I'd like some fun... |
| ham   | Even my brother is not like to speak with me. They treat me like aids patent.           |  

In this dataset:
- **ham**: Non-spam messages (e.g., social messages, personal conversations).
- **spam**: Spam messages (e.g., promotions, scams, unwanted advertisements).


## Steps Involved
### 1. **Data Cleaning**
- Removing irrelevant columns and renaming necessary columns for clarity.

### 2. **Exploratory Data Analysis (EDA)**
- Analyzing the distribution of spam and ham messages.
- Adding features like the number of characters, words, and sentences in each message.

### 3. **Data Preprocessing**
- Converting text to lowercase.
- Tokenizing the text and removing special characters, stopwords, and punctuation.
- Stemming words to their root form.

### 4. **Model Building**
- Using multiple machine learning algorithms like **Naive Bayes**, **Logistic Regression**, **SVM**, and **Random Forest** to train and evaluate the model.
  
### 5. **Model Evaluation**
- The models are evaluated using **accuracy**, **precision**, and **confusion matrix** to assess the performance.

## Model Evaluation
The model is evaluated based on:
- **Accuracy**: Percentage of correct predictions.
- **Precision**: Percentage of relevant results among the retrieved instances.

Here are some evaluation results:

| Model            | Accuracy   | Precision   |
|------------------|------------|-------------|
| **MultinomialNB**| 97.2%      | 100%        |
| **BernoulliNB**  | 98.3%      | 99.2%       |
| **SVC**          | 86.6%      | 0% (Precision issue with SVC) |

## How to Run
1. Clone this repository to your local machine.
2. Install the required libraries:
3. Run the Jupyter notebook (`sms-spam-detection.ipynb`) to see the results and model evaluation.

## Acknowledgments

Thank you for exploring this project! If you found this repository helpful or interesting, please consider giving it a ⭐. Contributions, suggestions, and improvements are always welcome. Feel free to open an issue or submit a pull request.
