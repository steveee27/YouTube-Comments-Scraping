# YouTube Comments Sentiment Analysis

This project involves scraping and analyzing YouTube comments from machine learning-related videos in Bahasa Indonesia. The comments are processed and analyzed using various text representation techniques to extract key insights about popular terms and themes.

## Table of Contents
- [Project Overview](#project-overview)
- [Project Workflow](#project-workflow)
- [Conclusion](#conclusion)
- [License](#license)

## Project Overview

- **Data Source**: YouTube comments on machine learning videos in Bahasa Indonesia.
- **Text Representation Techniques**: TF-IDF and Word2Vec (CBOW).
- **Analysis Methods**: Word frequency analysis and word cloud visualization.

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
4. **Analysis and Visualization**:
   - **Word Frequency Analysis**: Identified the most common terms in the comments.
   - **Word Cloud**: Visualized frequent words to reveal popular themes.

## Conclusion

This project demonstrates the process of collecting, processing, and analyzing text data from YouTube comments, highlighting various text representation techniques. Through word frequency analysis and word cloud visualization, we uncovered common themes and key terms discussed in the comments, such as "machine learning," "data," and "training." These insights provide an overview of popular topics in Indonesian-language machine learning discussions on YouTube.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
