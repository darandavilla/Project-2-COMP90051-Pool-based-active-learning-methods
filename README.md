# SML_COMP90051_S1_2021_Assignment2
Statistical Machine Learning UoM - Assignment 2 - S1 2021

Project 2: Implementing Active Learning methods

The goal of this project was to code a set of active learning algorithms using a logistic regression component classifier. The dataset used for this project was comprised of a matrix encoding images of handwritten characters and string valued labels that encoded the alphabet names of each image. The implemented algorithms were:

- Random Heuristic (Settles, 2012): Using a batched active learning framework using a random selection heuristic achieves around 50% of accuracy. This result could be improved by using other techniques for selecting samples to reveal their labels to the model.
- Uncertainty Sampling (Schein and Ungar, 2007): The uncertainty sampling method for active learning was used to select instances that have the most predictive uncertainty under the model. It was expected for this model to be slightly better than using the random selection heuristic, however, it reached about the same result. A better result could be obtained and a difference between the two strategies could be made if using more instances.
- Query by Committee (Settles, 2012): In general, using bagging with different measures of disagreement (hardvote entropy, softvote entropy and KL divergence) got better results compared to uncertainty sampling and random selection. Moreover, bagging was able to take several weak Logistic Regression models while aggregating their prediction and selecting the best predicions from those. Bagging brought better results as it queries the most informative instances, which makes the model more stable, reducing the variance and improving accuracy.



