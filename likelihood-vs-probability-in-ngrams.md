## Review: Continuous and Discrete Distributions

continuous have infinite values, uncountable, even if the range is finite (height or weight of people in class, think bell curve graph)
discrete are countable (number of customers in a store at a specific time, think bar graph).

a random variable is the result of an experiment or occurrence that is either part of a continuous or discrete distribution of possible events  that could have occurred

### Probability vs Likelihood in Continuous and Discrete Distributions

in a continuous distribution:
 - when we talk about probability, we know the parameters , such as the mean or mu of the probability density function, it is a conceptualisation and does not require an observation 
 
 - when we talk about likelihood, it is because we've made an observation, an event has occurred, however, in the real world, we don't actually know the parameters, we do however know the x value within the probability density function. 

in a discrete distribution:
 - when we talk about probability, we know the parameters, such as the bias of a coin flip (50% for example), is a conceptualisation and we can talk about what we will expect if we perform a coin flip with that exact parameter/bias, but we're not dealing with any observed data actually

 - when we talk about likelihood, an event has occurred, a coin has been flipped, we can't know the bias of the coin

## Probability vs Likelihood when dealing with N-grams

>when constructing a language model, our goal is to estimate the likelihood of unseen word sequences based on a corpus

in order to create that language model one technique is using ngrams when let's say we have a particular corpus as the training data

[i stopped here for now]

N-gram is a string of words of N length

we want to know the probability of that sequence in that order, i.e. its ngram probability

a particular sentence or string of words from a corpus has a particular, unknowable probability based on the underlying language model for example the model for any word sequence to appear in the english language. This underlying language model is practically unknowable due to the the sheer number of parameters and possible word sequences


ngram probability deals with discrete distribution by getting the counts of that particular ngram in the corpus that it came from



## Maximizing the likelihood:
