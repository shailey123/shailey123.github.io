## Perspectives on Unsupervised Deeplearning
 The supervised deep learnig problem has been solved to a fairly igh degree of effectiveness. However, the cost and difficulty of generating large volumes of labelled data represent a huge barrier to widespread deployment of these techniques to solve everyday problesm, business or otherwise. Increasingly the focus and emphasis of growth in deeplearning is shifting towards unsupervised learning. Examples of such applications include clustering similar examples, generating new examples, or determing how likely some point is. These kinds of tasks require some kind of unsupervised or semi supervised learning. 
 
 # Challenges with unspervised learning
 There are many challenges with unsupervised learning related to the high dimensionalityof teh random variables being modeled.  These can be broadly groued under two heads;
 1. Challenges related to statistical generalization: exponential increase in the number of statistical confiugrations with increase in dimensions
 2.The computional challenge due to the fact that many algorithms involve intractable computations that increase exponentially with number of dimensions. In partiucalr for probabilistic models this computational challege arises from the need to perfrom intractable inference or normalize the distribution
   * Intractable inference: Very simply , this is guessing the value of variable 'a', given other variable 'b', with respect to model that captures the joint distribution of 'a, 'b', 'c'. To compute such conditional proabilites requires one to sum over the values of variable 'c'.
   * Intractable normalization constants: Normalizing constants of probability functions come up in infreence as well as learning. This is related to partition fucntions. (NB: these are tough concepts. i could not find much at the googling level. Will come back and update when get more 'tractable' material!)
 
 The Goodfellow et al(2015) go onto dsicsus various ways in which current deeplearning research is overcoming these problesm.thier suggested approaches ilcude:
 1. Aprroximation of intractable computations
 2. Avoiding these computations by appropriately designing methods to avoid them


# References 

Goodfellow, Ian and Bengio, Yoshua and Courville, Aaron, (2016), 'Deep Learning', MIT Press

  
