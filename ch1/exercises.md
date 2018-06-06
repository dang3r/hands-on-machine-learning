# 1. How would you define machine learning?

Machine learning is when a program becomes more proficient the more data it
gets.

# 2. Can you name four types of problems where it shines:

1. Classification: Distinguishing between different cats and dogs, determing
   what emails are spam.
2. Regression: Predicting stock price data, housing prices
3. Clustering: Grouping different people
4. Anomaly Detection: Classifying fraud, bad physics particle data
5. Association Rule Learning: If certain people go to a certain store in a mall,
   they also go to another store.

# 3. What is a labelled training set?

A training set where each example has a label indicating what it maps to. An
example may be a picture of a tiger `P` is labelled `tiger` or an integer
mapping to tiger. Each label is the desired solution for the input.

# 4. What are the two most common supervised tasks?

1. Classification
2. Regression

# 5. Can you name 4 common unsupervised tasks?

1. Anomaly Detection
2. Clustering
3. Association Rule Learning
4. Visualization algorithms

# 6. What type of machine learning algorithm would you use to allow a robot to walk in various unknown terrains?

Reinforcement learning because:

- supervised learning means we would have to know what the right moves to make
  are in a given terrain. This would require a lot of walking or transportation
  data
- using reinforcement, robots can make a given move and if good, we positively
  reinforcem. Else, negative.

# 7. What type of algorithm would you use to segment your customers into different populations?

Unsupervised learning via clustering algorithms.

# 8. Would you frame the problem of spam detection as a supervised learning problem or an unsupervised learning problem?

I think you can try both, but supervised learning is better:

- we want to classify where an email is spam or not (it is binary). Getting
  labels to train on for existing emails isn't hard.
- we could cluster using an unsupervised algorithm. However, it may be possible
  that spam is spread into multiple clusters. If they are mixed in clusters with
  many regular emails, we don't gain much.

# 9. What is an online learning system?

An online learning system is one that learns incrementally on new data is
streamed in . An online leanring system can learn from new data as it comes in,
instead of being retrained periodically.

# 10. What is out of core learning?

When a machine learning algorithm is trained using data that cannot fit into a
machine's memory.

# 11. What type of machine learning algorithm relies on a similarity measure to make predictions?

Instance based learning. It has a similar metric that determines how similar an
example is to those it trained on.

# 12. What is the different between a model parameter and a learning algorithm's hyperparameter?

A hyperparameter is a parameter of the learning algorithm (learning rate)
whereas a model parameter can be a weight of an edge.

Model parameters are affected by the learning algorithm and the
hyperparameter(s) as a result.

# 13. What do model based learning-algorithms search for? What is the common strategy they use to succeed? How do they make predictions?

A model based learning algorithm searches for a function that uses input
attributes to predict the label or solution of a training example. They use
utility functions and cost functions to model parameters in order to improve
their predictive power. They make predictions by feeding an input to its model
which yields an output.

# 14. Can you name four of the main challenges in machine learning?

1. Not enough training data.
2. Irrelevant features. The features fed to the model are irrelevant to those
   required to make accurate predictions.
3. Overfitting. The machine leanring algorithm may not generalize to examples
   outside of the training set.
4. Underfitting. The learning algorithm is too simple to have predictive power.

# 15. If your model performs great on the training data but generalizes poorly to new instances, what is happening? name three possible solutions.

You are overfitting to the training data.

Three solutions are:

- Minimize the number of epochs you train your algorithm with. 
- Regularization. Restrict the exploration space for model parameters. Keep the
  model simple.
- Minimize noise in your data. Ensure the features you provide and the patterns
  in them are generalizable and not specific to the training set.

# 16. What is a test set and why would you want to use it?

It is a subset of the available training data reserved for validating the model
post-training. A typicaly rule is to use an 80:20 split for
training_data:test_data.
