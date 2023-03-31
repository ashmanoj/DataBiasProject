What I'm studying: I am assesing Google's Prespective API to see if it is biased in flagging comments as toxic based on the length of the comment

Hypothesis: The model will be biased against shorter comments, which means it will flag shorter comments as more toxic than longer comments.

Method: I created 2 lists for short and long comments. Each category has a predicted list and actual list, and I compared them to each other to evaluate the true negatives and true positives to calculate class 1 and class 2 accuracies. 


Results:

Class 1(toxic) accuracy for short comments is 0.8421052631578947
Class 0(nontoxic) accuracy for short comments is 0.9166666666666666
Class 1(toxic) accuracy for long comments is 0.6666666666666666
Class 0(nontoxic) accuracy for long comments is 1.0

it appears that the model's accuracy in predicting Class 1 (toxic) comments is lower for long comments compared to short comments. Specifically, the Class 1 accuracy is 0.842 for short comments but drops to 0.667 for long comments. This suggests that the model may be biased towards predicting Class 1 for shorter comments and may struggle to accurately classify longer comments as toxic.

Theories: I think the results were how they are maybe because people who leave shorter comments are more likely to write toxic comments. Also the testing sample was pretty small, which could have results in a baised result. 
