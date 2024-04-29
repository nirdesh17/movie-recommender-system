# Movie Recommendation System

This project focuses on building a movie recommendation system using AI/ML techniques. The system suggests similar movies based on user preferences, movie genres, keywords, cast, crew, and movie descriptions.

## Dataset
- The dataset used in this project consists of two CSV files:
    - `tmdb_5000_movies.csv`: Contains information about movies such as title, overview, genres, keywords, etc.
    - `tmdb_5000_credits.csv`: Contains information about movie credits including cast and crew details.

## Data Preprocessing
- **Merging**: The two datasets are merged using the movie titles as the common key.
- **Cleaning**: Null values are dropped and duplicates are removed from the merged dataset.
- **Feature Selection**: Selected features include title, overview, genres, keywords, cast, and crew.

## Feature Engineering
- **Data Transformation**: Certain columns containing JSON-formatted data (genres, keywords, cast, crew) are converted into lists.
- **Text Processing**: Textual data such as overviews, genres, keywords, cast names, and crew names are processed to remove spaces, convert to lowercase, and perform stemming.

## Vectorization
- **Count Vectorization**: The textual data is vectorized using CountVectorizer to convert it into numerical form.
- **Feature Extraction**: The most frequent words are selected as features, and their occurrences are counted.

## Similarity Calculation
- **Cosine Similarity**: Cosine similarity is calculated between vectors to measure the similarity between movies.
- **Recommendations**: Based on the similarity scores, top similar movies are recommended to the user.

## Implementation
- The recommendation function takes a movie title as input and suggests similar movies.
- **Visualization** (Optional): PCA is used for visualization of the vectorized data (commented out in the code).
- **Example Usage**: The **`recommend()`** function is called with a movie title to demonstrate how the system works.

## Technologies Used
- Python
- **Libraries**: Pandas, NumPy, NLTK, scikit-learn
- **Data Visualization**: Matplotlib (for optional visualization)


## Setup and Installation
- Install the required Python libraries (Pandas, NumPy, NLTK, scikit-learn).
- Download the dataset files (`tmdb_5000_movies.csv` and `tmdb_5000_credits.csv`).
- Run the provided code to preprocess the data, extract features, and build the recommendation system.
- Call the **`recommend()`** function with a movie title to get recommendations.



For any issues or improvements, please feel free to contribute or reach out.

### Connect me:
[Linkedin](https://www.linkedin.com/in/nirdesh-devadiya-55b408209)
