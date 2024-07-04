> Clarification of certain statistics terms and concepts

> **Resource that i have not yet checked out but looks good:**
> - Probability (Math): https://stats.libretexts.org/Courses/Saint_Mary's_College_Notre_Dame/MATH_345__-_Probability_(Kuter)

# Random Variables (Source: Gemini, https://youtu.be/3v9w79NhsfI, khan academy, https://www.youtube.com/watch?v=dOr0NKyD31Q)
- uncertain numerical outcome of an experiment or random process
- the quantification of outcomes in random processes
## **Discrete Random Variables:** 
Can only take on specific, separate values (like number of dots on a die). Probability focuses on individual values (e.g., probability of rolling a 3). could also be from an infinite set of possibilities but it would have to be **countable**
  - **mean (expected value)**: multiply the probabilities of the occurrences of each separate value occurring with their corresponding separate values and then add them together.

      - gives you an idea around which value outcomes will cluster, ex: dice rolls cluster around 3.5
      $$E = \sum_{i} (x_i \cdot p_i)$$

      **Explanation of the formula:** (Source: Gemini)

      * **$E$**: Represents the expected value (mean).
      * **$\sum_{i}$ (capital sigma summation):** Represents the sum over all possible values (i) of the variable.
      * **$x_i$**: Represents the i-th possible value of the variable. 
      * **$p_i$**: Represents the probability of pthe i-th value of the variable (p_i must be between 0 and 1, and the sum of all probabilities for all possipble values must equal 1).

## **Continuous Random Variables:** 
Can take on any value within a specific range (like height). Probability focuses on ranges (e.g., probability of being between 1.7m and 1.8m tall). any value in an interval even an infinite one. not countable, for example like the exact mass of a random animal, it is **uncountable** because the decimal places could keep going on forever. another example is the exact winning time of a race. 
  - can take on any value within a range
  - **mean (expected value)**: need to use the probability density function **pdf** and integration
      
      (Formula source: gemini)
      
      $$E = \int_{a}^{b} x \cdot f(x) \, dx$$

      **Explanation of the formula:**

      * **$E$**: Represents the expected value (mean).
      * **$\int_{a}^{b}$**: Represents the definite integral over a specific range from lower bound `a` to upper bound `b`. This range defines the possible values for the continuous random variable. 
          * In some cases, the range might be from negative infinity to positive infinity (represented by $-\infty$ and $\infty$ symbols), depending on the distribution.
      * **$x$**: Represents the value of the variable.
      * **$f(x)$**: Represents the probability density function (pdf) of the variable. The pdf defines the relative likelihood of different values for the variable.
      * **$dx$**: Represents the infinitesimal change in the variable during integration.

      **Key points to remember:**

      * This formula assumes the integral converges (meaning it has a finite value). Not all probability density functions have finite integrals. 
      * The specific range of integration (a to b) depends on the particular continuous distribution and its possible values.


## Probability Distributions

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
 - Of all those probabilities, one thing **must happen**
   - because a probability is the chance of something happening, specifically one thing
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
 - Likelihoods of a single outcome under multiple probability distributions do not add up to one.
  
In **normal distributions** (a type of continuous distribution):
 - probability = area under the curve
 - bell curve
 - each point on a normal distribution is a **probability density** but the probability of any point occurring is zero since there are infinite points
 - the probability density at any single point just indicates the **relative likelihood** of encountering a value in a small range around that point
 - the normal bell curve (with standard deviation 1) is described by the **density**:

> Formula, explanations, notes for the probability density function of a normal distribution provided by Google's Gemini AI

$$ f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{ -\frac{(x - \mu)^2}{2\sigma^2}} $$

**Explanation of the symbols:**

* `f(x)`: Represents the density function at a specific value `x`.
* `μ`: Represents the mean of the normal distribution.
* `σ`: Represents the standard deviation of the normal distribution.

**Notes:**

*  This formula describes the density function for any normal distribution, not just the standard normal distribution (where μ = 0 and σ = 1).

example:
suppose we observe x = 1
probability x = 1 is 0
density at x = 1 depends on which universe we are in, i.e. which normal distribution we have
for continuous distribution, the relevant question is not "what is a likelihood vs a probability", rather it is a **density vs likelihood**

>it is a probability density function if we view it as a function of x where  `μ` is known
>
>it is a likelihood function if we viewed as a function of the unknown parameter `μ`, where x is known

## breakdown from gemini ai to clarify:

**Probability vs. Likelihood:**

* **Probability:** Refers to the chance of a specific event happening within a given sample space. In the context of a continuous distribution with a known parameter (like μ, the mean), the pdf defines the probability density of different values (x) the variable can take on.
* **Likelihood:** Refers to the probability of observing a particular set of data (already observed) given a specific model or hypothesis. In this case, the likelihood function describes how well different possible values of the unknown parameter (like μ) explain the observed data (known x values).

**Key Differences:**

| Feature        | Probability (pdf) | Likelihood |
|----------------|-------------------|------------|
| Focus           | Probability density of different values (x) | How well a parameter (μ) explains observed data (x) |
| Parameter       | Known (e.g., μ) | Unknown (e.g., μ) |
| Data            | Not required (conceptual) | Observed (known x values) |

**Understanding the Viewpoints:**

* **PDF as a Function of x (known μ):** When you view the pdf as a function of x with a known parameter (μ), you're essentially focusing on the probability density for different possible values of the variable (x) given that specific value of μ. This helps understand the overall shape and behavior of the distribution for a fixed parameter.
* **Likelihood Function (unknown μ):** When you consider the likelihood function, the focus shifts to explaining observed data (known x values). You have different possible values for the unknown parameter (μ) and calculate the likelihood (how well each μ explains the observed data). Techniques like maximum likelihood estimation aim to find the μ value that maximizes this likelihood.

**Observation and the PDF:**

While it might seem like no observation has occurred when considering the pdf as a function of x, it's not entirely accurate. The pdf itself is based on the underlying theoretical distribution and its parameters (like μ). It represents the probability density for any possible value (x) **if** the distribution holds true. We don't necessarily need a specific observation (known x value) to define the pdf, but it's based on the characteristics of the distribution itself.

**Think of it this way:** Imagine a coin toss. The probability of heads (p) is a fixed parameter. You can define the probability density for heads and tails (0.5 each) without actually flipping a coin. However, if you already flipped the coin and observed heads, the likelihood function would focus on how well different possible values of p (between 0 and 1) explain the observed outcome of heads.

**In essence, the distinction between probability and likelihood hinges on whether you're interested in the general probability density for different values within a known distribution (pdf) or the relative fit of different parameters to explain observed data (likelihood function).**
