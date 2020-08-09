# What are Linear Factor models?
Chapter 13, Deep Learning, basically deals with something called Linear Factor models. these are probabilitic models based on 'latent' variables. i meediately run into a problem: what are 'latent' variables? so, that's goign to be quite a divagation. But, before I do that let me just try and summarize the motivation for Linear Factor Models. If the Latent variables takes too much time, i will set up a separate post for it. 

The Deep Learning book says:
" Linear factor models are some of the simples probabilitic models models with latent variables".
Appraently these models also form the basis of the approach used to develop Generative models, hence probably can't be skipped, unfortunately! Okay, spoiler alert: at this point, pretty well third paragraph of Ch 13, things start to get pretty heavy. From here on English is abandoned in favour of difficult mathematical notation. Here is where I come in: I shall attempt to decode this maths as far as I can. Be warned: at some point, descent into maths syntax is inevitable. 

A simpler explanation of latent variables picked up from Stefano Ermon's Stanford course on Probabilistic Graphical Models(CS228) - see references below. FYI this is the simplest explanation I could find after about 15 mintues of surfing. Other articles included 'gated' Medium articles and some papers on Arxiv. 

In a normal probabilitic model, we learn a fucntion, g(x,y), based on two explcit variables, x, and y. For example a probabilitic model of news articles will have words, and sentences as your x and y. However each news article also represents a topic represented by t, for example, finace, sports, etc. Now we can build a more accurate model, g(x,y|t).p(t) which also takes into account t. Note as of now t is unobserved, but we are calling out that it exists. 

# References
1. https://ermongroup.github.io/cs228-notes/learning/latent/
