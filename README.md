# 🎬 Movies Recommendation System using Machine Learning  

A machine learning-based movie recommender that helps users discover new films by analyzing **genres, keywords, cast, and directors**.  
This project demonstrates how **Content-Based Filtering** can be implemented using NLP techniques and similarity measures.  

---

## 🚀 Features
- 🔍 **Content-Based Recommendations** → Suggests movies similar to what you like.  
- 🎭 **Feature Engineering** → Uses genre, cast, crew, and keywords for personalization.  
- 📊 **Vectorization** → TF-IDF / CountVectorizer to convert text into meaningful vectors.  
- 📐 **Cosine Similarity** → Measures similarity between movies to generate recommendations.  
- 🌐 **User Interface** → Simple web app (`app.py`) built using Streamlit/Flask for easy interaction.  

---

## 📂 Dataset
The system uses TMDB datasets:  
- `tmdb_5000_movies.csv` → Movie details (title, genres, overview, etc.)  
- `tmdb_5000_credits.csv` → Cast and crew details  

Both datasets are merged on **movie ID** for a complete feature set.  

---

## 🛠️ Tech Stack
- **Python 3.8+**  
- **Pandas, NumPy** → Data wrangling  
- **Scikit-learn** → Vectorization & similarity computation  
- **NLTK / re** → Text preprocessing  
- **Flask / Streamlit** → Web interface  

---

## 📌 Workflow
1. **Data Preprocessing** → Clean and merge movie + credits dataset.  
2. **Feature Selection** → Extract genres, keywords, cast, and director.  
3. **Text Vectorization** → Convert text into vectors using TF-IDF or CountVectorizer.  
4. **Similarity Calculation** → Compute similarity matrix with cosine similarity.  
5. **Recommendation Engine** → Input a movie → return top N similar movies.  
6. **Deployment** → Run `app.py` to use the interactive web app.  
