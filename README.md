# Movies-Recommendation-System-using-ML

Overview of the Movies Recommendation System using Machine Learning implemented in the provided notebook:

# 1. Content-Based Recommendation System:
• Objective: This system recommends movies to users based on the content of the movies they have liked in the past.<br/>
• Approach: The system uses movie features such as genre, keywords, cast, and director to find similar movies.
# 2. Data Loading and Preprocessing:
• The code loads two datasets:<br/>
    -->tmdb_5000_movies.csv: Contains details about movies like title, genres, overview, etc.<br/>
    -->tmdb_5000_credits.csv: Includes information about the movie cast and crew.<br/>
These datasets are merged based on the movie ID to combine all relevant information.
# 3. Feature Selection:
•The model extracts key features such as:<br/>
    -->Genres (e.g., Action, Comedy)<br/>
    -->Keywords (e.g., Adventure, Hero)<br/>
    -->Cast (main actors/actresses)<br/>
    -->Director (who directed the movie)<br/>
These features are combined to create a single text vector for each movie.
# 4. Text Vectorization and Similarity Calculation:
• The combined text is vectorized using TF-IDF or CountVectorizer to transform text data into numerical format.<br/>
• Cosine Similarity measures the similarity between movie vectorized representations. It calculates how similar two movies are based on their feature vectors.
# 5. Recommendation Function:
• When a user inputs a movie title, the system:<br/>
    -->Find the movie in the dataset.<br/>
    -->Retrieves its vector representation.<br/>
    -->Computes the cosine similarity between this movie and all other movies.<br/>
    -->Returns a list of the most similar movies as recommendations.
# 6. User Interface (app.py):
• The app.py file likely contains a simple web application (using frameworks like Streamlit or Flask). Users can input a movie title and receive recommendations through a user-friendly interface.
