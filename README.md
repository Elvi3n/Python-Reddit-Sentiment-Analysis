# Python-Reddit-Sentiment-Analysis

Sentiment analysis on Reddit posts using the PRAW library for scraping and the VADER SentimentIntensityAnalyzer for text analysis. The analysis is presented in a Jupyter Notebook.

```
Project Structure
├── data/                       # (optional) storage for datasets  
├── LICENSE                     # license file  
├── README.md                   # project documentation  
├── Reddit_Sentiment_Analysis.ipynb  # main notebook  
└── requirements.txt            # Python dependencies  
```

## Setup

- python -m venv .venv
- source .venv/bin/activate   # macOS/Linux
- .venv\Scripts\activate      # Windows


### Install the required packages:

pip install -r requirements.txt

*Reddit API credentials are required. Create a Reddit app by following the OAuth2 Quick Start Guide*
. Update your client ID, client secret, and user agent in the notebook before running.

## Workflow

- Web Scraping:

- Collects posts from a target subreddit using PRAW.

  - Stores titles, bodies, and URLs in a structured DataFrame.

- Sentiment Analysis:

  - Applies VADER to calculate negative, neutral, positive, and compound scores.

  - Stores sentiment scores in the DataFrame.

## Findings

Highest sentiment score (positive): 0.99
Lowest sentiment score (negative): -0.99

### Distribution Plot

The histogram below shows that posts cluster in the pettyrevenge subreddiit at the extremes. Meaning the subreddit’s content is polarized: people either narrate their stories with deep negativity or with triumphant positivity, likely from their success in taking revenge. The lack of middle-ground suggests that revenge stories are emotionally charged by nature.

<img width="562" height="455" alt="output" src="https://github.com/user-attachments/assets/e8298b90-57f7-4312-bb40-a699d546ca77" />

## License

This project is licensed under the terms of the LICENSE file included in the repository.
