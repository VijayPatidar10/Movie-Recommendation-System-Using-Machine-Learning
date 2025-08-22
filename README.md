# Movie-Recommendation-System-Using-Machine-Learning

A content-based movie recommendation system built using Python and machine learning. This project suggests movies to users based on their favorite movie.

## How It Works
The recommendation system is built on the principle of "content-based filtering." It recommends movies that are similar in content to the one the user likes. The process is as follows:

**Data Collection:** The project uses a dataset of movies (movies.csv) which contains various features for each film.

**Feature Selection:** Key content features are selected for the recommendation model. These include:

genres

keywords

tagline

cast

director

**Data Preprocessing:** The selected features are combined into a single string for each movie. Any missing data in these columns is filled with an empty string.

**Text Vectorization:** The combined text data is converted into a matrix of TF-IDF features. TfidfVectorizer is used to quantify the importance of each word in the documents.

**Similarity Calculation:** Cosine similarity is used to calculate a numeric similarity score between all movies based on their feature vectors.

**Recommendation:** When a user enters a movie title, the system finds its closest match in the dataset and then provides a sorted list of the most similar movies based on their cosine similarity scores.

## Technologies Used
**Python**

**Pandas:** For data manipulation and analysis.

**NumPy:** For numerical operations.

**Scikit-learn:** For implementing TF-IDF Vectorizer and Cosine Similarity.

**Difflib:** For finding the closest match to the user's input movie title.

**Jupyter Notebook:** For interactive development and presentation.

## How to Run
Ensure you have Python and Jupyter Notebook installed.

Clone this repository to your local machine.

Install the required libraries.

Run the MovieRecommendationUsingMachineLearning.ipynb notebook.

Follow the prompt to enter your favorite movie name and receive a list of recommended movies.
