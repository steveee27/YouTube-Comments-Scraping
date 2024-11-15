# YouTube Comments Sentiment Analysis

This project involves scraping and analyzing YouTube comments from machine learning-related videos in Bahasa Indonesia. The comments are processed and analyzed using various text representation techniques to extract key insights about popular terms and themes.

## Table of Contents
- [Project Overview](#project-overview)
- [Project Workflow](#project-workflow)
- [Results](#results)
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
   - **Word Cloud**: Visualized the frequent words to reveal popular themes.

## Results

| Text Representation | Analysis | Key Findings |
|---------------------|----------|--------------|
| **TF-IDF**          | Word Frequency Analysis | Identified key terms such as "machine learning", "data", "training", etc. |
| **Word2Vec (CBOW)** | Word Cloud | Visualized terms related to learning and data processing, showing the popularity of specific topics in comments. |

## Conclusion

This project demonstrates the process of collecting, processing, and analyzing text data from YouTube comments, showcasing various text representation techniques. The analysis provides insights into key terms and themes discussed in machine learning content on YouTube in Bahasa Indonesia.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
