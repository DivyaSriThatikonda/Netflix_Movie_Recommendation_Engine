# Netflix_Movie_Recommendation_Engine

**Personalized Movie Recommendation System using SVD(Singular Value Decomposition)**

**Project Overview:**

The goal of this project is to develop a personalized movie recommendation system using Singular Value Decomposition (SVD). By

analyzing user ratings from the "combined_data.txt" file and movie data from the "movie_titles.csv" file, the system will 

generate tailored movie recommendations for individual users based on their viewing history and preferences.

**Dataset:**

**Movie Titles Data:** Contains information about movie titles and release years.

**User Ratings Data:** Includes user ratings for various movies.

    
**Singular Value Decomposition (SVD):**

SVD is a matrix factorization technique used to decompose a matrix into three separate matrices, representing latent factors

that capture underlying patterns in the data. In the context of recommendation systems, SVD is applied to the user-item rating 

matrix to extract latent features and generate personalized recommendations.

Singular Value Decomposition (SVD) is a fundamental matrix factorization technique used in various fields such as linear

algebra, signal processing, and machine learning. It decomposes a matrix into three separate matrices, capturing underlying 

patterns and relationships within the data.

The SVD decomposition of a matrix AA is represented as:

A=UΣV^T

Where:

U=U is an orthogonal matrix containing the left singular vectors.

Σ=SigmaΣ is a diagonal matrix containing the singular values.
 
V^T=V^Tis the transpose of an orthogonal matrix containing the right singular vectors.

## Installation

To run the project in your Jupyter Notebook or Google Colab, follow these steps:

1. **Clone the repository**:
   - If using Jupyter Notebook:
     ```bash
     !git clone https://github.com/DivyaSriThatikonda/Netflix_Movie_Recommendation_Engine.git
     ```
   - If using Google Colab:
     - Open a new Colab notebook.
     - Execute the following code cell:
       ```python
       !git clone https://github.com/DivyaSriThatikonda/Netflix_Movie_Recommendation_Engine.git
       ```
2. **Install dependencies**:
   - Run the following code cell in the notebook to install the required libraries:
     ```python
     !pip install numpy pandas matplotlib seaborn scikit-learn
     ```

3. **Access the dataset**:
   - The `insurance.csv` dataset is already included in the repository. 

4.**Tools used**:
- **Numpy**: Used for numerical computations and array manipulation.
- 
- **Pandas**: Used for data manipulation, analysis, and cleaning.
- 
- **Seaborn**: Used for data visualization and statistical plotting.
- 
- **Scikit-learn**: Used for building and evaluating the linear regression model.
- 
- **Descriptive Statistics**: Used to summarize and analyze the dataset, including measures such as mean, median, standard deviation, and correlation coefficients.
- 
- **Matplotlib**:Used for data visualization

 # Results
       Year                                            Name         Estimate_Score
4352  2002.0                  Curb Your Enthusiasm: Season 3        5.000000
2018  2004.0                                Samurai Champloo        5.000000
721   2003.0                              The Wire: Season 1        5.000000
241   1995.0  Neon Genesis Evangelion: The End of Evangelion        5.000000
871   1954.0                                   Seven Samurai        5.000000
174   1992.0                                  Reservoir Dogs        5.000000
2101  1994.0                          The Simpsons: Season 6        4.994354
4114  1999.0                         The Simpsons: Bart Wars        4.972430
2429  1979.0                      Alien: Collector's Edition        4.970744
404   1987.0                                 Wings of Desire        4.952919

Singular Value Decomposition (SVD) model is trained on the movie ratings dataset and then predicted the above ratings for movies 

for user with user_id = 1 has not yet rated and recommended the top 10 movies with the highest predicted ratings to this user.

The output displays the recommended movies along with their release years and estimated scores. These are the movies that the 

SVD model suggests would be highly rated by the user with user_id = 1, based on their preferences and past ratings.
