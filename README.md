# 🎬 IMDb & TMDb Movie Analysis Project

This project extracts, cleans, and analyzes movie data from **IMDb** and **TMDb**, combining both sources to explore patterns in user sentiment, ratings, and box office performance.

## 📌 Objectives

- Scrape IMDb movie reviews (Top 100) using `BeautifulSoup`.
- Collect movie revenue and ratings from TMDb using their API.
- Clean and merge both datasets on movie names.
- Analyze sentiment, ratings, and revenue to answer key business questions.

---

## 🔍 Data Sources

- **IMDb**: https://www.imdb.com/chart/top  
  Used to extract top-rated movie reviews.
  
- **TMDb API**: https://developer.themoviedb.org/reference/intro/getting-started  
  Used to fetch movie revenue and vote averages.

---

## 📁 Project Structure
```bash
movie-analysis/
│
├── data/ # All CSV outputs
│ ├── Reviews.csvSS
│ ├── Revenue.csv
│ ├── q1.csv # Avg rating & review count per movie
│ ├── q2.csv # Sentiment category per movie
│ └── q3.csv # Sentiment vs revenue & rating
│
├── notebooks/
│ └── imdb_tmdb_analysis.ipynb
│
├── .env # Contains TMDb API key (NOT uploaded)
├── .gitignore
├── requirements.txt
└── README.md
```


## 💡 Key Questions Answered

1. **What is the average user rating and review count for each movie?**
2. **What is the sentiment category (positive/neutral/negative) for each movie?**
3. **How does sentiment affect total revenue and average rating across movies?**
4. **Which movies are underperforming (high user rating but low revenue)?**
5. **What are the top-rated and top-grossing movies in the dataset?**

---

## 📊 Tools & Libraries Used

- `requests`, `BeautifulSoup` — Web scraping
- `pandas` — Data manipulation
- `textblob` — Sentiment analysis
- `matplotlib`, `wordcloud` — Visualization
- `python-dotenv` — API key management

---

## 🛠️ How to Run This Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/movie-analysis.git
cd movie-analysis
```
---
### 2. Set Up Virtual Environment (Optional but Recommended)

```bash
python -m venv .venv
.\.venv\Scripts\activate   # Windows
```
---

### 3. Install Required Libraries
```bash
pip install -r requirements.txt
```
---

### 4. Set Up Your .env File
```bash
TMDB_API_KEY=your_tmdb_api_key_here
```
---

### Run the Notebook
Navigate to the notebooks/ folder and open:
```bash
imdb_tmdb_analysis.ipynb
```
### 🔒 Security Note
Your API key is stored in a .env file, which is excluded from GitHub using .gitignore. Never commit your .env or API keys.

### 📌 Sample Results (CSV Outputs)
    q1.csv – Ratings & review counts
    q2.csv – Sentiment classification
    q3.csv – Sentiment vs Revenue vs Ratings

### 📬 Contact
Feel free to reach out if you have suggestions or questions.
