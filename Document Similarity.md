layout: page
title: "Document Similarity in NLP and Text Mining"
permalink: /https://github.com/shailey123/shailey123.github.io/
## Document Similarity in NLP and Text Mining
One of the biggest challenges in NLP and text mining is understanding and deriving insight from large volumes of txt data. One way of doing this is via document similarity. Document similarity enables matching of one document with another. This can be broken down into matching of a search query with a document, matching two queries with each other or matching documents. It can also be used an an input to rank documents. A key challenge with similarity measures is that there is no one accepted 'best' measure. Each meansure comes with its pros and cons and scenarios where it can be used. 

The following meausres are available:

1. Precsion, recall and F1 Score
2. Dice coefficient
3. Jaccard Coefficient
4. Cosine Similarity
5. Asymmetric Similarity
6. Euclidean distance
7. Manhattan Blocks Distance 
Let's take each of thes and try and understand what they mean. The next few sections are going to be mathematical, but I will try and decode it a bit.

#Precsion, recall and F Score
We begin with something that you are would be quite familiar with. Precision, recall and F Scores are frequently used metrics in a range of supervised classification tasks. Precision in the context of classification is the True Positive/(True Positives + False Positives). It is usually taken as a measure of the accuracy of you forecast, i.e., out of all my predictions, how many of them have I predicted accurately. Recall is the reverse. It measures out of all my Positives, how many have I been able to predict accurately, i.e., True Positives/(True Positives + False Negatives). An example of its application to information retrieval: suppoe a search query leads to 30 pages being retrieved and out of these 20 are relevant. Further there is another 40 pages which are relevant that were not retieved. The Precision is 20/30=.66, Recall is 20/60 = .33 . According to wikipedia page on Precision and Recall: precision is "_how useful the search results are_", and recall is "_how complete the results are_".

![image](https://user-images.githubusercontent.com/37128883/88649678-b4f0f580-d0e5-11ea-81c8-cad7a263695a.png)

![image](https://user-images.githubusercontent.com/37128883/88649050-2ed4af00-d0e5-11ea-8d1f-3c77a0d4e2ad.png)

The F Score is the harmoic mean of Precision and Recall scores. 
The formula for F1 score is: F1 Score = 2(Precision* Recall)/(Precision + Recall)
The FI Score represents the balance between Precsion and Recall. It is used extensively in information retrieval for document classification and matching. A challenge with F1 Score is that it gives equal weightage of both Precision and Recall whereas the relative importance of these might differ depending on the problem. 

##References
https://machinelearningmastery.com/classification-accuracy-is-not-enough-more-performance-measures-you-can-use/
https://en.wikipedia.org/wiki/Precision_and_recall
https://en.wikipedia.org/wiki/F1_score
http://eacharya.inflibnet.ac.in/data-server/eacharya-documents/53e0c6cbe413016f23443704_INFIEP_33/18/LM/33-18-LM-V1-S1__document_similarity_measures.pdf
