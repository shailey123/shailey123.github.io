# What are Linear Factor models?
Chapter 13, Deep Learning, basically deals with something called Linear Factor models. these are probabilitic models based on 'latent' variables. i immediately run into a problem: what are 'latent' variables? so, that's goign to be quite a divagation. But, before I do that let me just try and summarize the motivation for Linear Factor Models. If the Latent variables takes too much time, i will set up a separate post for it. 

The Deep Learning book says:
" Linear factor models are some of the simple probabilitic models models with latent variables".
Apparently these models also form the basis of the approach used to develop Generative models, hence probably can't be skipped, unfortunately! Okay, spoiler alert: at this point, pretty well third paragraph of Ch 13, things start to get pretty heavy. From here on English is abandoned in favour of difficult mathematical notation. Here is where I come in: I shall attempt to decode this maths as far as I can. Be warned: at some point, descent into maths syntax is inevitable. 

A simpler explanation of latent variables picked up from Stefano Ermon's Stanford course on Probabilistic Graphical Models(CS228) - see references below. FYI this is the simplest explanation I could find after about 15 mintues of surfing. Other articles included 'gated' Medium articles and some papers on Arxiv. 

In a normal probabilitic model, we learn a fucntion, g(x,y), based on two explcit variables, x, and y. For example a probabilitic model of news articles will have words, and sentences as your x and y. However each news article also represents a topic represented by t, for example, finace, sports, etc. Now we can build a more accurate model, g(x,y|t).p(t) which also takes into account t. Note as of now t is unobserved, but we are calling out that it exists. This approach is more accurate becasue we ca learn a separate function, g(x,y|t) for each t. This is better than trying to learn a catchall g(x,y) across all categories. However, since t is unobserved the method of learning t becomes more complex. 

So, how are LMVs useful in machine learning. There are two reasons:
1. They enable us to leverage our prior knowledge: For example in the topic modeling example, LMVs enable us t o know that T diffrent topics and hence probility distributions exist in the corpus. 
2. LMVs, more tacticlly, can also be used to help replace missing data. For example in the case of clinical trials, if some respondents drop out, then LVMs can be used to model their responses on dquestions that they did not answer. 

That was the last part part that I could find acrss muliple readings that is in English. Going forward it is algebra.
Status check: completely overcome by waves of sleep, a clear warning that things are looking very tough!

First let me overview the techniques that are there in this chapter:

1. Proabilitic PCA and Factor Analysis
2. Independent components Analysis 
3. Slow Feature analysis ( Never heard of it)
4. Sparse coding 
5. Manisfold intrpretation of PCA

Okay first up:

## Linear Factor Model
Explained in a slightly complex way. But simply, it is that an observed variable x is a linear compination of independent latent factors, h. 
x= Wh + b+ noise

 h ∼ p(h)
 
 Now the 5 models that I listed above, most of these use this linear factor model adn different assumptins for noise or the way we model the prior function, p(h).

# References
1. https://ermongroup.github.io/cs228-notes/learning/latent/
