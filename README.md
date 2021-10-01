# FakeNewsDetection

PROBLEM STATEMENT

Fake news is misleading information spread to damage the reputation of a person/identity or making money through advertising revenue.
It is generally spread through social media using honeycomb framework and the third-person effect hypothesis, people usually forward it ahead without checking its authenticity.
Often the outcome of this can be dreadful resulting into riots, mob killings and other forms of violence.
Research shows that 1 in 2 Indians receives fake news via WhatsApp and Facebook as per a survey by Social Media Matters and Institute for Governance, Policies and Politics we can be 
fooled or manipulated- into worsening existing stereotypes, getting worried about fake disease 
epidemics, or even influencing whom we vote for.

Reference -https://www.slideshare.net/HarshdaGhai/fake-news-detection-project.

METHODOLOGY

IMPLEMENTATION DETAILS

First, take a news data that will contain text, label, title, etc. Label can 
be in any form either 0 and 1 or fake and real. On the basis of this news 
data, we will predict. After taking data set first, we will analyze it 
because data set text content very large amount of text that will 
consume very large memory, to resolve we will have to remove it's all 
stop word. We will also remove the data that contain empty column 
now we will have to divide the data set into two parts, first is training 
part and second is testing part. We will take this data in any ratio like 
80% and 20% .80% will be our training part and 20% will be our testing 
part. Now by using TF-IDF vectorizer, we convert the text of testing part 
and training part into a meaningful number then we have to use 
Passive Aggressive classifier four reaction that is the news is fake or not. 
This algorithm reacts positive for the true data and react aggressive for 
fake data, we have to predict it on testing part. Now from this step we 
will get total number of predictions that will be true. Thus, from this 
data we will get accuracy score. Accuracy score = (total true positive + 
total true negative) / (total true positive + total false positive + total 
false negative + total true negative) This accuracy score will give us that 
how much data is accurate we can also read confusion matrix 
*Confusion matrix = [ TP FP FN TN]

Data

Data link : https://www.kaggle.com/c/fake-news/data (because of large size we can not upload on github)

We are using dataset from kaggle.com which contains the following features:
id:  id for a news article
title: the title of a news article
author: author of the news article
text: the text of the article
label: a label that marks the article as potentially unreliable
Real: unreliable
Fake: reliable

Data preprocessing -

Remove special characters from text ,Spell checked all the documents ,Remove the Stop Words from the documents.





Model----


We use TfIdf Vectorizer to convert our text  to numerical representations and initialize a PassiveAgressive Classifier to fit the model.

 Tf-Idf Vectorizer is a common algorithm to transform text into meaningful representation of numbers. It is used to extract features from text strings based on occurrence.
We assume that higher number of repetitions of a word would mean greater importance in the given text.

 Passive Aggressive classifier -. This algorithm react positive for the true data and react aggressive for fake data , we have to predict it on testing part.

 In the end, the accuracy score and confusion matrix tell us how well our model works.
 Passive Aggressive classifier -. This algorithm react positive for the true data and react aggressive for fake data , we have to predict it on testing part.

 In the end, the accuracy score and confusion matrix tell us how well our model works .





SCOPE OF IMPROVEMENT

This project could have been made more user-friendly, as most of the users are active through their mobile phones the scope of making a better android friendly interface was always there. It is still functional on mobile phones but going into much more detail, testing and tweaking it, refining it at every stage was always possible.

Also, the datasets which we got were of comparatively smaller size, if we could have larger datasets then it would have been even better as it would have increased the accuracy of the model substantially and the possibility of using more graphs and tables to analyze and elaborate the result in a better way was also present



REFERENCE

https://towardsdatascience.com/fake-news-detection-with-machine-

https://www.indiaspend.com/manipulative-fake-news-on-the-rise-in-

https://www.kaggle.com/c/fake-news/data
