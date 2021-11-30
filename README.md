# Triplet networks and One-shot learning


#### Part of Assignment of Deep Learning Course (2IMM10) at TU/e 


## Objective

In practice 4b.4, we train a Siamese network for one-shot learning task on the Omniglot dataset. 

In this assignment, we will work on the same data set with the same task but extend it to triplet networks, we will also compare our model performance under different triplet selection method.

The assignment contains the following 4 tasks.

### Task 1: Build the triplet network

When training the model, make sure the network achieves a smaller loss than the margin and the network does not collapse all representations to zero vectors.

### Task 2: Define triplet loss

When training the model, make sure the network achieves a smaller loss than the margin and the network does not collapse all representations to zero vectors.

### Task 3: Select triplets for training

We have two different options for the triplet selection method, and we will compare the model performance under these two selection methods after building our model

a. Random triplets selection, including the following steps:
	* Pick one random class for anchor.
	* Pick two different random picture for this class, as the anchor and positive images.
	* Pick another class for Negative, different from anchor class.
	* Pick one random picture from the negative class.
b.  Hard triplets selection. For easy implement, for a picked anchor, positive pair, we will choose the hardest negative to form a hard triplet, that means, after picking an anchor, positive image, we will choose the negative image which is nearest from anchor image from a negative class, i.e : distance between anchor image and negative image can get the minimum value. The whole process including the following steps:

	* Pick one random class for anchor.
	* Pick two different random picture for this class, as the anchor and positive images.
	* Pick another class for Negative, different from anchor class.
	* Pick one hardest picture from the negative class.
	

### Task 4: One-shot learning with different selection method

With different triplets selecting method (random and hard), we will train our model and evaluate the model by one-shot learning accuracy.

* You need to explicitly state the accuracy under different triplets selecting method

* When evaluating model with test oneshot function, you should evaluate on 20 way one-shot task, and set the number (k) of evaluation one-shot tasks to be 250, then calculate the average accuracy




