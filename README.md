# Movie Recommendation System (TMDB 5000 Dataset)

## Overview

This repository contains the implementation of a content-based movie recommendation system using the **TMDB 5000 Movie Dataset**. The project leverages feature extraction techniques such as TF-IDF vectorization on movie descriptions and genre analysis to recommend similar movies based on the input movie.

## Approach

1. **Data Preprocessing**  
   The dataset is first cleaned by removing duplicates and handling missing data, particularly in the movie descriptions. 

2. **Feature Representation**  
   - **Handmade Features**: Movie genres are extracted and used to represent the movie's category.
   - **Non-Handmade Features**: TF-IDF vectorization is applied to the movie descriptions to extract semantic similarities between movies.

3. **Model Selection**  
   A **content-based recommendation** approach is used, as it focuses on the intrinsic properties of movies (e.g., genres and descriptions). This method does not require user interaction data, making it suitable for datasets where user data is limited or unavailable.

4. **Cosine Similarity**  
   The recommendation is based on the cosine similarity measure between movies' feature vectors. Given a movie title, the system returns the top 5 most similar movies.

5. **Visualization**  
   Data visualizations are used to explore movie properties, such as the distribution of movie ratings, revenue, and popularity, along with the frequency of different genres in the dataset.

## Getting Started

### Prerequisites

To run this project locally, you need the following:

- Python 3.x
- Required Python libraries:  
  - pandas  
  - numpy  
  - scikit-learn  
  - matplotlib  
  - seaborn

You can install these dependencies using pip:

```bash
pip install -r requirements.txt
