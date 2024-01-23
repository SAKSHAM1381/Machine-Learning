# Machine-Learning
A project made by a group of 3 as a part of Coursework. 

# Description of the project
A simple yet challenging project, to anticipate the quality of wine. The com-
plexity arises due to the fact that the data set has fewer samples is highly
imbalanced. Can you overcome these obstacles build a good predictive model
to classify them? Features in the data set are continuous but all have dif-
ferent ranges, so we normalized them by dividing with the respective maximum
of each feature which reduces the range between 0 and 1. Now that we have a
normalized data set we have used Machine Learning model, in this case random
forest, which is a ensemble model which creates decision trees. Random forest
is a versatile, convenient machine learning technique that, in most cases, gives
good results even without hyper-parameter adjustment. Due to its simplicity
and adaptability, it is also one of the most widely used algorithms it can be used
for both classification and regression tasks, so we have used the random forest
classifier for our project.

# Experiments
First we tried to use Support Vector Machine (SVM) model but due to the
different ranges of the features accuracy turned out to be just 50 percent which
was not good. Later we tried decision tree classifier but because of lots of data
the overfitting has occured and the pruning method made the problem more
complicated which gave only 58 . We also tried Random forest and decision tree
but there were so many features that meant lots of unstructured data so even
with this model we got only 66 percentage of accuracy. As there were different
ranges in the features we tried to classify them with KNN but even with the
KNN we could not find ideal k-value for the data set and the best accuracy
we got is 61 percent. Finally we have used Random Forest Classifier which gave
us the highest accuracy of 76 percent. We have trained the model on previously
normalized data set, we used the similar data set to predict the model by
splitting 25 percentage of the data set for testing and 75 percentage for training.
To do this we have used sklearn’s train test split method by setting the shuffle
attribute to true and random state to 0.33

# Conclusion
Using the ML models, we have analyzed which of the features were contributing
more to the result and which were not and we have predicted quality of the wine
which turned out be 76 percent. We introduced the RF as a machine learning
classifiers to predict wine quality after evaluating its performance based on the
accuracy,precision, recall, F1 scores, the ROC-AUC score. According to the
results, AdaBoost predicted wine quality with higher accuracy during without
feature selection, with feature selection and with essential variables. Overall,
performance of all classifiers (except KNN) improved when model trained and
tested using essential variables. The usefulness of data generation algorithms
and importance of feature selection is the key feature in this study. We are in
progress of developing a machine learning-based web application that wine
researchers and wine growers can use to predict wine quality based on the
important available chemical and physiochemical compounds in their wines,
one that has the capability to tune various variable quantities.

# Machine-Learning
A project made by a group of 2 as a part of Coursework.

# Description of the project
To develop a basic recommendation system using Python and Pandas. 
Emphasis on providing a basic recommendation system by suggesting items that are most similar to a particular item, in this case, movies. It just tells what movies/items are most similar to the user’s movie choice.

# Approaches to build Recommender Systems
 There are two main types of recommendation engines
1. Collaborative Filtering
2.  Content-Based Filtering.

Collaborative filtering is calculated only on the basis of the rating a user gives to an item. For example, two users can be considered similar if they give the same ratings to ten movies To find the rating R that a user U would give to an item I, the approach includes:
1. Finding users similar to U who have rated the item I
2. Calculating the ratingRbased the ratings of users found in the previous step
   
 Content based filtering uses item features to recommend other items similar to what the user likes, based on their previous actions or explicit feedback.
1. It uses the similarity metrics which is calculated from the item’s feature vectors and the user’s preferred feature vectors from his/her previous records.
2. Then, the top few are recommended.
