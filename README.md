# Understanding_customer_review_with_NLP

Project summary

Yelp is a local business review network.  Every day thousands of customers wrote comments to express their thoughts on a wide range of products and services. It is critical for a merchant to understand what their customer like or dislike from these review comments.
In this project, I have two major goals. First, I built language understanding models that determine whether a comment is positive or negative. This will be done by both supervised and unsupervised learning. Next, I built restaurant recommendation system based on customer preference.


Data resource

Yelp Dataset Challenge Round 12


Challenges and solutions

•	Representation of unstructured review text. Three major strategies were performed to convert text into numerical vector machine can used. First, I generated features represent text composition such as text length and number of question/exclamation marks. Secondly, term-document matrix was constructed that each text was represented by TF-IDF score, which reveal occurrence statistics. Thirdly, I trained embedding from my train data and compared its effect on classification model with the pre-trained word embedding of Word2Vec skip-gram and GloVe. Fourthly, I integrated my samples with embedding weights from feed-forward Neural-Net Language Models in TensorFlow Hub. 
•	Architecture of deep neural network.  I selected LSTM, GRU, bidirectional LSTM/GRU for classification models. A series of experiments were performed to determine how model performance were dependent on layer depth and width, combination of diverse layer and dropout rate.
