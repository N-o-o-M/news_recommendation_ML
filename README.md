# News Recommendation System Based on Mood and Interests

## Overview
This project is a news recommendation system that scrapes the latest news articles from a website, processes them using natural language processing (NLP), and recommends relevant articles based on user mood and interests. It utilizes web scraping, text embeddings, and clustering for personalized recommendations.

## Features
- **Web Scraping**: Extracts latest news articles from `indianexpress.com`
- **NLP Embeddings**: Uses `SentenceTransformer` to generate text embeddings
- **Clustering**: Implements K-Means clustering to group articles into topics
- **Personalized Recommendations**: Suggests articles based on user mood and interests
- **Cosine Similarity Matching**: Finds articles most relevant to user preferences

## Technologies Used
- **Python** (Core language)
- **BeautifulSoup** (Web scraping)
- **Requests** (Fetching web pages)
- **Pandas** (Data manipulation)
- **SentenceTransformer** (Text embeddings)
- **Scikit-learn (KMeans, Cosine Similarity)** (Clustering and similarity calculations)

## Installation
### Clone the repository:

### Install dependencies:
```sh
pip install requests beautifulsoup4 pandas scikit-learn sentence-transformers
```

## Usage
### 1. Scraping News Articles
Run the following script to scrape news articles:
```sh
python main.py
```
This fetches the latest articles from `indianexpress.com` and processes them.

### 2. Getting Personalized Recommendations
- Enter your **mood** (e.g., happy, curious, serious)
- Provide your **interests** (comma-separated, e.g., technology, politics, health)
- The system will return **top 10 recommended articles**

#### Example Interaction:
```sh
Enter your mood (e.g., happy, curious, serious): curious
Enter your interests, separated by commas: technology, AI, innovation
```

#### Example Output:
```
Title: AI Revolution in 2025
URL: https://example.com/ai-revolution-2025
Description: How artificial intelligence is changing the world.
Date: Jan 29, 2025
Topic: 3
```

## Future Enhancements
- Improve clustering by experimenting with different algorithms
- Incorporate sentiment analysis to refine mood-based recommendations
- Deploy as a web app using Flask or FastAPI
- Add more news sources for diverse article recommendations

---
**Contributions are welcome!** If you find any issues or want to enhance the system, feel free to open a pull request.

