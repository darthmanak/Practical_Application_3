In this project, we are going to examine the performance of different classifiers that we have learned. The classifiers that will be examined are K 
Nearest Neighbors, Logistic Regression, Decision Trees, and Support Vector Machines. To do so, we will use a dataset that contains several bank telephone 
marketing campaigns that were done by a Portuguese banking institution and whether are not the bank successfully was able to get the person they called to 
subscribe a term deposit. Here is the link to the dataset. 

The table view of the database where I stored the performance of the different classifiers can be seen in model_results.

As we can see, there is not much difference in terms of the train accuracy and the test accuracy. Almost all of these tests had a score of 0.87 which means 
that it is pretty accurate. It took Support Vector Machines a lot more time to train the dataset than it did with the others as SVM took 11 seconds whereas 
the others took much less than a single second. 

There are several more improvements that could be made to this assignment. One that I tested for myself was if we plugged in different k-values to see 
which accuracy was the highest. Aa graphical representation of the different k-values and their accuracies can be seen in different_k.
  
While the scores plateau around when k=11, the highest score is recorded when k=25. However, when k was 25, even though the test accuracy was a bit 
higher, the train accuracy was a bit lower. Below are the results of when k=25 and my original KNN test where k=1.

				K = 25  		K = 1 		 Difference
	Train Accuracy  	0.873436543339456	0.876017	-0.002580250153065622
	Test Accuracy		0.8737864077669902	0.863815	0.009971136184728335
	
This makes this theory inconclusive as some K’s yield better test accuracies while yielding worse train accuracies and vice versa.
Some other improvements that I could have made is using a GridSearch to find the most optimal parameters for each of the four classifiers and testing the 
results that they give off. During the actual tests, I ran the default parameters for all of the classifiers. There are many parameters that could be 
changed for the better. I believe that this would significantly help with improving the training time for SVM. Another improvement could be whether we
include gender as one of the features that are involved. I believe that this should be tested for because it could change the outcome and score possibility
of whether the person being called submits a term deposit. 
        
Link to the Jupyter Notebook with my work is here: http://localhost:8888/lab/tree/Downloads/module_17_starter/prompt_III.ipynb
