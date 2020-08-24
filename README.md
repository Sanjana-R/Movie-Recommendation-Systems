# Movie Recommendation Systems
Three movie recommendation systems using 1) K-Nearest Neighbour Algorithm, 2) Correlation Analysis and 3) Matrix Factorization. 

## Details 

### - Setup Details
Jupyter notebook

Python

SciPy library

NumPy

Scikit-learn

Pandas

Fuzzywuzzy

### - About the Dataset
Movielens Dataset: https://grouplens.org/datasets/movielens/100k/

This dataset consists of:
* 100,000 ratings (1-5) from 943 users on 1682 movies.
* Each user has rated at least 20 movies.
* Simple demographic info for the users (age, gender, occupation, zip)
MovieID::Title::Genres
- Titles are identical to titles provided by the IMDB (including
year of release)
- Genres are pipe-separated and are selected from the following genres:
  * Action
  * Adventure
  * Animation
  * Children's
  * Comedy
  * Crime
  * Documentary
  * Drama
  * Fantasy
  * Film-Noir
  * Horror
  * Musical
  * Mystery
  * Romance
  * Sci-Fi
  * Thriller
  * War
  * Western
  
  ### - Evaluation Metrics
  As we have used unsupervised learning in these recommender systems, we do not have the
necessary data of class labels in order to accurately and easily predict accuracy, precision,
recall, and f-measure.

● Accuracy refers to the ratio of correct predictions made.

    ○ (# Correct Predictions) / (Total # of samples)

● Precision identifies the proportion of correct positive identifications

    ○ (True Positives) / (True Positives+False Positives)
    
● Recall is the proportion of actual positives identified correctly

    ○ (True Positives) / (True Positives+False Negative)
    
● F1 measure is the weighted harmonic mean between precision and recall

    ○ (2*Precision*Recall) / (Precision+Recall)
    
## Conclusion
We have explored three different, simple algorithms for collaborative filtering-based movie
recommendation systems. 

- Correlation Analysis identifies the relation between rankings of a
watched movie and every other movie in the system. 

- KNN finds movies with the least distance (most similarity) to the watched movie. 
- Matrix Factorization identifies movies that hold a similarity with the list of movies that the user has previously viewed, resulting in a more
personalized list with more inter-list dissimilarity.

Although none of the algorithms yield perfect results, they may be combined into a more
complex recommender system, through the use of an ensemble. Ensemble learning allows the
usage of all of these algorithms to be incorporated into a single one with higher performance.
One such possible system could be:

- KNN takes a watched movie as input and outputs a list of related movies

- Matrix Factorization takes a user as input and outputs a list of movies similar to what the
user has viewed in the past.

- On a streaming platform, a user with an account ID who has previously watched a movie
can be recommended a list of movies based on the majority of the movies offered in both
algorithms. This would yield higher accuracy, as it satisfies the requirements of movie similarity
and personalization.

Another possible system could take the output of the KNN model as an input to the SVD model
and further filter the recommendation based on the user’s preferences, using Matrix
Factorization.
  
  
## Contributors
Sanjana Rai

Naveena Koneru 

## References
https://www.github.com/SaurusXI/Movie-Recommender

https://www.ee.columbia.edu/~cylin/course/bigdata/EECS6893-BigDataAnalytics-Lecture4.pdf

https://towardsdatascience.com/how-to-build-from-scratch-a-content-based-movie-recommender-with-natural-language-processing-25ad400eb243

https://www.dezyre.com/data-science-in-python-tutorial/principal-component-analysis-tutorial

https://blog.imarticus.org/data-analytics-popular-algorithms-explained/

https://www.analyticsvidhya.com/blog/2018/06/comprehensive-guide-recommendation-engine-python/

https://towardsdatascience.com/evaluation-metrics-for-recommender-systems-df56c6611093

https://grouplens.org/datasets/movielens/

https://towardsdatascience.com/ensemble-methods-in-machine-learning-what-are-they-and-why-use-them-68ec3f9fef5f

https://medium.com/greyatom/decision-trees-a-simple-way-to-visualize-a-decision-dc506a403aeb

https://towardsdatascience.com/machine-learning-basics-with-the-k-nearest-neighbors-algorithm-6a6e71d01761


