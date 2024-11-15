# YouTube Comments Sentiment Analysis

This project involves scraping and analyzing YouTube comments from machine learning-related videos in Bahasa Indonesia. The comments are processed and analyzed using various machine learning algorithms and text representation techniques to extract key insights.

## Table of Contents
- [Project Overview](#project-overview)
- [Project Workflow](#project-workflow)
- [Results](#results)
- [Conclusion](#conclusion)
- [License](#license)

## Project Overview

- **Data Source**: YouTube comments on machine learning videos in Bahasa Indonesia.
- **Text Representation Techniques**: TF-IDF and Word2Vec (CBOW).
- **Machine Learning Algorithms**: Support Vector Machine (SVM) and Random Forest.
- **Performance Metrics**: Accuracy, Precision, Recall, and F1 Score.

## Project Workflow

1. **Data Collection**: Comments were scraped from YouTube using the YouTube API.
2. **Data Preprocessing**: 
   - Cleansing: Removed irrelevant text, emojis, and special characters.
   - Tokenization: Split comments into individual words.
   - Stopword Removal: Removed common stopwords to focus on relevant words.
   - Lemmatization: Reduced words to their base forms.
3. **Text Representation**:
   - **TF-IDF**: Term Frequency-Inverse Document Frequency to represent text as a numerical feature vector.
   - **Word2Vec (CBOW)**: Continuous Bag of Words for capturing semantic similarity between words.
4. **Modeling and Evaluation**:
   - **Algorithms**: SVM and Random Forest were applied with default settings and hyperparameter tuning.
   - **Evaluation**: Models were evaluated on accuracy, precision, recall, and F1 score.

## Results

| Text Representation | Algorithm | Hyperparameters | Accuracy | Precision | Recall | F1 Score |
|---------------------|-----------|-----------------|----------|-----------|--------|----------|
| **TF-IDF (Default)** | **SVM** | c = 1.0, kernel = rbf, gamma = scale | 0.9547 | 0.9553 | 0.9547 | 0.9547 |
|  | SVM (Tuning 1) | c = 0.5, kernel = linear, gamma = auto | 0.9544 | 0.9546 | 0.9544 | 0.9543 |
|  | SVM (Tuning 2) | c = 1.5, kernel = poly, gamma = scale | 0.8346 | 0.8783 | 0.8346 | 0.8357 |
|  | **Random Forest** | n_estimators = 100, max_depth = None, min_samples_split = 2 | 0.9345 | 0.9338 | 0.9345 | 0.9344 |
|  | Random Forest (Tuning 1) | n_estimators = 150, max_depth = 20, min_samples_split = 5 | 0.8140 | 0.8630 | 0.8140 | 0.8140 |
|  | Random Forest (Tuning 2) | n_estimators = 50, max_depth = 50, min_samples_split = 3 | 0.9218 | 0.9260 | 0.9218 | 0.9216 |
| **TF-IDF (Tuned)**<br> min_df = 5, max_df = 0.95 | **SVM** | c = 1.0, kernel = rbf, gamma = scale | **0.9551** | **0.9556** | **0.9551** | **0.9551** |
|  | Random Forest | n_estimators = 100, max_depth = None, min_samples_split = 2 | 0.9361 | 0.9376 | 0.9361 | 0.9360 |
| **Word2Vec (CBOW)** | **SVM** | c = 1.0, kernel = rbf, gamma = scale | 0.9290 | 0.9292 | 0.9290 | 0.9289 |
|  | SVM (Tuning 1) | c = 1.5, kernel = linear, gamma = scale | 0.9298 | 0.9298 | 0.9298 | 0.9297 |
|  | SVM (Tuning 2) | c = 0.5, kernel = poly, gamma = auto | 0.8544 | 0.8567 | 0.8544 | 0.8526 |
|  | **Random Forest** | n_estimators = 100, max_depth = None, min_samples_split = 2 | 0.9405 | 0.9406 | 0.9405 | 0.9405 |
|  | Random Forest (Tuning 1) | n_estimators = 75, max_depth = 45, min_samples_split = 4 | **0.9425** | **0.9426** | **0.9425** | **0.9424** |
|  | Random Forest (Tuning 2) | n_estimators = 200, max_depth = 25, min_samples_split = 5 | 0.9406 | 0.9406 | 0.9406 | 0.9406 |

**Notes**:
- Hyperparameter tuning was performed to optimize the models for higher accuracy and F1 scores.
- The **SVM model with TF-IDF (Tuned)** and **Random Forest with Word2Vec (CBOW)** achieved the best performance overall.

## Conclusion

This project demonstrates the process of collecting, processing, and analyzing text data from YouTube comments, showcasing various text representation techniques and machine learning models. The results provide insights into key terms and themes discussed in machine learning content on YouTube in Bahasa Indonesia.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
