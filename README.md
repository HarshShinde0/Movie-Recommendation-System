This script recommends movies similar to a user’s favorite movie by analyzing content-based features. It follows these key steps:

Data Loading & Preprocessing:
Loads a dataset of 4,803 movies and selects relevant features (genres, keywords, tagline, cast, and director). Missing values are filled with empty strings.

Feature Combination:
Combines the selected textual features into a single string for each movie.

TF-IDF Vectorization:
Converts the combined text into numerical feature vectors using TfidfVectorizer.

Similarity Calculation:
Calculates cosine similarity between all pairs of movie vectors to measure content similarity.

User Input & Matching:
Accepts a movie title (hardcoded or passed programmatically due to Jupyter’s lack of input() support), finds the closest matching title, and retrieves its index.

Recommendation Output:
Sorts all other movies based on similarity score and prints the top 10 most similar movies.
