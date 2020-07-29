## d-tree

#### This is from an undergrad ML course assignment. Instructions:

Introduction
>Implement the ID3 decision tree learning algorithm that we discussed in class. To simplify the implementation, your system only needs to handle binary classification tasks (i.e. each instance will have a class value of 0 or 1). In addition, you may assume that all attributes are binary-valued (i.e. the only possible attribute values are 0 and 1) and that there are no missing values in the training or test data.
<br/><br/>
A sample training file (train.dat) and test file (test.dat) are provided. In these files, only lines containing non-space characters are relevant. The first relevant line holds the attribute names. Each following relevant line defines a single example. Each column holds this example’s value for the attribute named at the head of the column. The last unlabeled column holds the class label for the examples. In all of the following experiments, you should use this last class attribute to help train the tree and to determine whether a tree classifies an example correctly.
<br/><br/>
When building a decision tree, if you reach a leaf node but still have examples that belong to different classes, then choose the most frequent class (among the instances at the leaf node). If you reach a leaf node in the decision tree and have no examples left or the examples are equally split among multiple classes, then choose the class that is most frequent in the entire training set. You DO NOT need to implement pruning.
<br/><br/>
IMPORTANT: Don’t forget to use logarithm base 2 when computing entropy and set 0*log2 0 to 0.

a.	Build a decision tree using the training instances and print the tree in the same format as the example tree shown below.

b.	Use the learned decision tree to classify the training instances. Print the accuracy of the tree. (In this case, the tree has been trained and tested on the same data set.) The accuracy should be computed as the percentage of examples that were correctly classified. For example, if 86 of 90 examples are classified correctly, then the accuracy of the decision tree would be 95.6%. E.g.,

> Accuracy on training set (90 instances):

c.	Use the learned decision tree to classify the test instances. Print the accuracy of the tree. (In this case, the decision tree has been trained and tested on different data sets.) E.g.,

> Accuracy on test set (10 instances):

d.	Now, we want to investigate how the amount of training data affects the accuracy of the resulting decision tree. Plot a learning curve (i.e., a graph of the accuracy of your algorithm on the test set against different training set sizes) by re-training your learning algorithm using training set sizes of 100, 200, 300, . . ., 800. Briefly comment on the shape of the curve. Does it exhibit the usual properties of a learning curve?
