
# 🎬 Movie Recommender System

A Content-Based Movie Recommendation System built using Python and Machine Learning. This project suggests movies similar to a user's choice based on genres, keywords, and plot overviews.

## 🚀 Overview
As an Electrical Engineering student with a pre-medical background, I developed this system to explore the intersection of data science and software development. The system uses **Natural Language Processing (NLP)** to process movie metadata and suggest the top 5 most similar movies.

## 🛠️ Features
- **Data Cleaning:** Handled missing values and preprocessed JSON-formatted metadata.
- **Stemming:** Used NLTK's PorterStemmer to normalize words (e.g., 'actor' and 'actors' become the same).
- **Vectorization:** Converted text tags into 5,000-dimensional vectors using `CountVectorizer`.
- **Similarity Engine:** Utilized **Cosine Similarity** to calculate the mathematical distance between movie vectors.

## 💻 Tech Stack
- **Languages:** Python
- **Libraries:** Pandas, NumPy, Scikit-learn, NLTK
- **Frontend:** Streamlit (in progress)

## 📊 How it Works
1. Data is fetched from the TMDB 5000 Movies dataset.
2. A 'tags' column is created by merging genres, keywords, and overview.
3. Text is converted to vectors (Bag of Words).
4. **Cosine Similarity** is applied:
   $$\text{similarity} = \cos(\theta) = \frac{A \cdot B}{\|A\| \|B\|}$$
5. The top 5 closest vectors are recommended.

## 📂 Project Structure
- `movie_system.ipynb`: The main logic and preprocessing.
- `movie_dict.pkl`: Serialized movie data.
- `similarity.pkl`: Calculated similarity matrix (Not uploaded due to size).
