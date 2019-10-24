# Recommendation-System-on-MovieLens
In this repository we are going to introduce the reader to recommender systems. We will also build a simple recommender system in Python. The system is no where close to industry standards and is only meant as an introduction to recommender systems. We assume that the reader has prior experience with scientific packages such as pandas and numpy.\
 
 
 
## What is a recommender system?
A recommender system is a simple algorithm whose aim is to provide the most relevant information to a user by discovering patterns in a dataset. The algorithm rates the items and shows the user the items that they would rate highly. An example of recommendation in action is when you visit Amazon and you notice that some items are being recommended to you or when Netflix recommends certain movies to you. They are also used by Music streaming applications such as Spotify and Deezer to recommend music that you might like.\
 \
 \
Below is a very simple illustration of how recommender systems work in the context of an e-commerce site.
![illustration](https://github.com/Radtchinko/Recommendation-System-on-MovieLens/blob/master/WHAT%20IS%20A%20RECOMMENDER%20SYSTEM.png)
 \
Two users buy the same items A and B from an ecommerce store. When this happens the similarity index of these two users is computed. Depending on the score the system can recommend item C to the other user because it detects that those two users are similar in terms of the items they purchase.\
 
 
## Different types of recommendation engines
The most common types of recommendation systems are content based and **collaborative filtering** recommender systems. In collaborative filtering the behavior of a group of users is used to make recommendations to other users. Recommendation is based on the preference of other users. A simple example would be recommending a movie to a user based on the fact that their friend liked the movie.There are two types of collaborative models **Memory-based** methods and **Model-based methods**.The advantage of memory-based techniques is that they are simple to implement and the resulting recommendations are often easy to explain. They are divided into two:\
 \
**User-based collaborative filtering:** In this model products are recommended to a user based on the fact that the products have been liked by users similar to the user. For example if Derrick and Dennis like the same movies and a new movie comes out that Derick likes,then we can recommend that movie to Dennis because Derrick and Dennis seem to like the same movies.\
 \
**Item-based collaborative filtering:** These systems identify similar items based on users’ previous ratings. For example if users A,B and C gave a 5 star rating to books X and Y then when a user D buys book Y they also get a recommendation to purchase book X because the system identifies book X and Y as similar based on the ratings of users A,B and C.\
 \
**Model-based** methods are based on [matrix factorization](https://en.wikipedia.org/wiki/Non-negative_matrix_factorization) and are better at dealing with [sparsity](https://en.wikipedia.org/wiki/Sparse_matrix). They are developed using data mining, machine learning algorithms to predict users’ rating of unrated items. In this approach techniques such as [dimensionality reduction](https://en.wikipedia.org/wiki/Dimensionality_reduction) are used to improve the accuracy. Examples of such model-based methods include [decision trees](https://en.wikipedia.org/wiki/Decision_tree), [rule-based models](https://en.wikipedia.org/wiki/Rule-based_modeling), [Bayesian methods](https://en.wikipedia.org/wiki/Bayesian_inference) and latent factor models.\
 \
**Content based systems** use meta data such as genre, producer, actor, musician to recommend items say movies or music. Such a recommendation would be for instance recommending Infinity War that featured Vin Disiel because someone watched and liked The Fate of the Furious. Similarly you can get music recommendations from certain artists because you liked their music. Content based systems are based on the idea that if you liked a certain item you are most likely to like something that is similar to it.\
 
## Datasets to use for building recommender systems
In this tutorial we are going to use the [MovieLes Dataset](https://grouplens.org/datasets/movielens/). This dataset was put together by the Grouplens research group at the University of Minnesota. It contains 1, 10, and 20 million ratings. Movielens also has a website where you can sign up, contribute reviews and get movie recommendations. You can find more datasets for various data science task from [Dataquest’s data resource](https://www.dataquest.io/blog/free-datasets-for-projects/).
