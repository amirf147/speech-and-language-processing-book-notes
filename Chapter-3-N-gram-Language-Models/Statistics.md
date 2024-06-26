## Clarification of certain statistics terms and concepts

### Discrete probability distributions
>The information for this section is sourced from Google's Gemini AI

Discrete probability distributions describe the likelihood of various **countable outcomes** in a random event.  Here's a breakdown of the key points:

* **Discrete:**  This refers to outcomes that can be separated into distinct, individual values.  Imagine counting something - the number of times you roll a die (1, 2, 3, 4, 5, or 6), the number of customers in a store at a specific time (0, 1, 2, 3, etc.), or the number of successes in a fixed number of trials (e.g., getting heads 3 times in 5 coin flips). These are all examples of discrete outcomes.

* **Probability Distribution:** This refers to a mathematical framework that shows the probability (chance) of each possible outcome occurring.  Imagine a graph where each outcome has a corresponding bar representing how likely it is.  The higher the bar, the more probable that outcome.

**Key characteristics of discrete probability distributions:**

1. **Finite or countable outcomes:** There must be a finite number of possible outcomes, or at least they must be countable (e.g., the number of people living in a city).
2. **Probabilities between 0 and 1:** The probability of any outcome must be between 0 (impossible) and 1 (certain).
3. **Sum of probabilities equals 1:** The sum of the probabilities for all possible outcomes must add up to 1.  This ensures all possibilities are covered.

**Examples of Discrete Probability Distributions:**

* **Binomial Distribution:** Used for calculating the probability of success in a fixed number of trials (e.g., flipping a coin 10 times and getting heads 3 times).
* **Poisson Distribution:** Used for modeling the number of events occurring in a fixed interval of time or space (e.g., the number of customer complaints received in a day).
* **Geometric Distribution:** Used for calculating the probability of the first success occurring after a certain number of failures (e.g., the number of times you roll a die until you get a 6).

By understanding discrete probability distributions, you can analyze the likelihood of various outcomes in situations with countable possibilities. This is useful in various fields like statistics, finance, games, and other applications where chance plays a role.

### Probability Vs. Likelihood
>Source for the following information, most of which is copied verbatim: [YouTube: Brian Greco - Learn Statistics! Probability vs. Likelihood ... MADE EASY!!!](https://www.youtube.com/watch?v=bXGjQnpGGIo)

In the context of **discrete probability distributions** (like coin flips):
 - Probability exists in **one universe**
 - A probability of an event is related to other events that occur in the same universe
 - The probabilities within the universe must all add up to 1
 - Of all those probabilities, one thing **must happen** (clarify?)
 - In probability, we know the _parameters_ which exactly describe the situation and how often things occur
 - Probability and likelihood are really the same thing, from different perspectives
 - Probability =  we know which universe we are in, and the probabilities of all events in that one universe add up to 1.
 - "**In statistics, we often do not know which universe we are in**"
   - "We only observed data, but we don't understand the process that created the data"

 - In likelihood we don't know the characteristics of the situation and how often things occur, we don't know what universe we are in
 - Different probabilities from different scenarios are likelihoods of our observed data under different scenarios
 - likelihoods are sometimes the **exact same numbers** as probabilities 
   - the term comes from the **context**
 - Likelihoods are a probability of the **observed data** under a hypothetical scenario. many hypothetical different scenarios, there are many likelihoods and they can't add up to one and thus cannot be interpreted as probabilities
 - Likelihood = we know what we observed, and we consider the probability of **what we observed** in any possible universe. 
  
In **normal distributions** (a type of continuous distribution):
 - probability = area under the curve