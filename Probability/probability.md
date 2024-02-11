# Probability

## Terminology

1. Random Experiment

    - An experiment is called random experiment if it satisfies the following two conditions:
        1. It has more than one possible outcome.
        2. It is not possible to predict the outcome in advance.

2. Trial

    - Trial refers to a single execution of a random experiment.
    - Each trial produces an outcome.

3. Outcome

    - Outcome refers to a single possible result of a trial.

4. Sample Space

    - Sample Space of a random experiment is the set of all possible outcomes that can occur.
    - Generally, one random experiment will have one set of sample space.

5. Event

    - Event is a specific set of outcomes from a random experiment or process.
    - Essentially, it's a
    subset of the sample space.
    - An event can include a single outcome, or it can include multiple outcomes.
    - One random experiments can have multiple events.

Example:

1. Random Experiment : randomly drawing out a passenger
2. Trial : finding its pclass
3. Outcome : 1
4. Sample Space : {1, 2, 3}
5. Event :
    1. The passenger is from pclass 2. {2}
    2. The passenger is not from pclass 2.
    {1, 3}

## Types of Events

1. Simple Event:
    - Also known as an elementary event, a simple event is an event that consists of exactly one outcome.
    - For example, when rolling a fair six-sided die, getting a 3 is a simple event.

2. Compound Event:
    - A compound event consists of two or more simple events.
    - For example, when rolling a die, the event "rolling an odd number" is a compound event because it consists of three simple events: rolling a 1, rolling a 3, or rolling a 5.

3. Independent Events:
    - Two events are independent if the occurrence of one event does not affect the probability of the occurrence of the other event.
    - For example, if you flip a coin and roll a die, the outcome of the coin flip does not affect the outcome of the die roll.

4. Dependent Events:
    - Events are dependent if the occurrence of one event does affect the probability of the occurrence of the other event.
    - For example, if you draw two cards from a deck without replacement, the outcome of the first draw affects the outcome of the second draw because there are fewer cards left in the deck.

5. Mutually Exclusive Events:
    - Two events are mutually exclusive (or disjoint) if they cannot both occur at the same time.
    - For example, when rolling a die, the events "roll a 2" and "roll a 4" are mutually exclusive because a single roll of the die cannot result in both a 2 and a 4.

6. Exhaustive Events:
    - A set of events is exhaustive if at least one of the events must occur when the experiment is performed.
    - For example, when rolling a die, the events "roll an even number" and "roll an odd number" are exhaustive because one or the other must occur on any roll.

7. Impossible event
    - It is an event that cannot occur under any circumstances, and its probability is assigned as 0.

8. Certain Event
    - It is an event that is guaranteed to occur, and its probability is assigned as 1.

## What is Probability

- In simplest terms, probability is a measure of the likelihood that a particular event will occur.
- It is a fundamental concept in statistics and is used to make predictions and informed decisions in a wide range of disciplines, including science, engineering, medicine, economics, and social sciences.
- Probability is usually expressed as a number between 0 and 1, inclusive:

  - A probability of 0 means that an event will not happen.
  - A probability of 1 means that an event will certainly happen.
  - A probability of 0.5 means that an event will happen half the time (or that it is as likely to happen as not to happen).

## Empirical Probability

- Empirical probability, also known as experimental probability, is a probability measure that is
based on observed data, rather than theoretical assumptions.
- It's calculated as the ratio of the number of times a particular event occurs to the total number of trials.

- Suppose that, in our 100 tosses, we get heads 55 times and tails 45 times.
- What is the empirical probability of getting a head. 55/100
- Let's say you have a bag with 50 marbles. Out of these 50 marbles, 20 are red, 15 are blue, and 15 are green.
- You start to draw marbles one at a time, replacing the marble back into the bag after each draw.
- After 200 draws, you find that you've drawn a red marble 80 times, a blue marble 70 times, and a green marble 50 times.
- What is the empirical probability of getting a red marble? 80/200

## Theoretical Probability

- Theoretical (or classical) probability is used when each outcome in a sample space is equally
likely to occur.
- Consider a scenario of tossing a fair coin 3 times. Find the probability of getting exactly 2 heads.
- Consider a scenario of rolling 2 dice. What is the probability of getting a sum = 7

1. Probability of an Event:

   $$P(A) = \frac{\text{Number of Favorable Outcomes}}{\text{Total Number of Possible Outcomes}}$$

2. Probability of the Complement of an Event:

   $$P(A') = 1 - P(A)$$

3. Probability of the Intersection of Independent Events:

   $$P(A \cap B) = P(A) \cdot P(B)$$

4. Probability of the Union of Events:

   $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

5. Joint Probability

    $$P(A \cap B) = P(A|B) \cdot P(B)$$

6. Marginal Probability

    $$P(A) = \sum_{i} P(A \cap B_i)$$

7. Conditional Probability:

   $$P(A|B) = \frac{P(A \cap B)}{P(B)}$$

8. Total Probability:

    $$P(A) = \sum_{i} P(A|B_i) \cdot P(B_i)$$

## Random Variable

- In the context of probability theory, a random variable is a function that maps the
outcomes of a random process (known as the sample space) to a set of real numbers.
- Input: The input to the function is an outcome from the sample space of a random
process.
- Output: The output of the function is a real number that we assign to each possible
outcome.
- The transformation from input to output in the function of a random variable is
determined by how we choose to define the random variable.
- The choice of how to define a random variable often depends on the specific aspects
of the random process (or event) that you're interested in studying.

## Probability Distribution of a Random Variable

- A probability distribution is a list of all of the possible outcomes of a random variable along
with their corresponding probability values.

| X    | 1    | 2    | 3    | 4    | 5    | 6    |
|------|------|------|------|------|------|------|
| P(X) | 1/6  | 1/6  | 1/6  | 1/6  | 1/6  | 1/6  |

- In this example, "X" is a discrete random variable because it takes on a finite number of distinct values (1, 2, 3, 4, 5, 6), and each value has an associated probability.

- This random variable "X" can be used to compute various probabilities and statistics related to Event , such as the expected value (mean) of the outcomes, variance, and more.

## Mean of a Random Variable

The mean of a random variable, often called the expected value, is essentially the average
outcome of a random process that is repeated many times. More technically, it's a weighted
average of the possible outcomes of the random variable, where each outcome is weighted by
its probability of occurrence.

For a discrete random variable X:
$$
E[X] = x_1 \cdot P(X = x_1) + x_2 \cdot P(X = x_2) + \ldots + x_n \cdot P(X = x_n)
$$

For a continuous random variable X:
$$
E[X] = \int_{x_{\text{range}}} x \cdot f(x) \, dx
$$

## Variance of a Random Variable

The variance of a random variable is a statistical measurement that describes how much
individual observations in a group differ from the mean (expected value).

For a discrete random variable X:
$$
\text{Var}(X) = (x_1 - E[X])^2 \cdot P(X = x_1) + (x_2 - E[X])^2 \cdot P(X = x_2) + \ldots + (x_n - E[X])^2 \cdot P(X = x_n)
$$

For a continuous random variable X:
$$
\text{Var}(X) = \int_{x_{\text{range}}} (x - E[X])^2 \cdot f(x) \, dx
$$

Let's consider a simple example of a discrete random variable representing the outcome of rolling a fair six-sided die. We'll calculate the mean (expected value) and variance for this random variable.

Example: Rolling a Fair Six-Sided Die

- For a fair six-sided die, the possible outcomes are: 1, 2, 3, 4, 5, 6.
- Each outcome has a probability of 1/6 since the die is fair.

1. Mean (Expected Value):

    - Using the formula for the mean of a discrete random variable:

    $$
    \
    E[X] = x_1 \cdot P(X = x_1) + x_2 \cdot P(X = x_2) + \ldots + x_n \cdot P(X = x_n)
    \
    $$

    $$
    \
    E[X] = 1 \cdot \frac{1}{6} + 2 \cdot \frac{1}{6} + 3 \cdot \frac{1}{6} + 4 \cdot \frac{1}{6} + 5 \cdot \frac{1}{6} + 6 \cdot \frac{1}{6} = \frac{21}{6} = 3.5
    \
    $$

    - So, the mean (expected value) of the random variable representing the outcome of rolling a fair six-sided die is 3.5.

2. Variance:

   - Using the formula for the variance of a discrete random variable:

   $$
   \
   \text{Var}(X) = (x_1 - E[X])^2 \cdot P(X = x_1) + (x_2 - E[X])^2 \cdot P(X = x_2) + \ldots + (x_n - E[X])^2 \cdot P(X = x_n)
   \
   $$

   $$
   \
   \text{Var}(X) = (1 - 3.5)^2 \cdot \frac{1}{6} + (2 - 3.5)^2 \cdot \frac{1}{6} + \ldots + (6 - 3.5)^2 \cdot \frac{1}{6} = \frac{35}{12} \approx 2.92
   \
   $$

   - So, the variance of the random variable representing the outcome of rolling a fair six-sided die is approximately 2.92.

- In this example, we calculated the mean and variance for a simple discrete random variable representing the outcomes of rolling a fair six-sided die.

## Venn Diagrams & Contingency Tables

- Venn diagrams and contingency tables are graphical and tabular tools used in probability and statistics to visualize and analyze relationships between different events, outcomes, or groups.
- They are particularly useful when dealing with multiple variables and their intersections. Let's take a closer look at each of them:

1. Venn Diagrams:

    - A Venn diagram is a visual representation of the relationships between different sets or groups.
    - In probability, Venn diagrams are commonly used to illustrate the intersections and unions of events.

    In a Venn diagram:

    - Circles represent sets or events.
    - Overlapping regions represent the intersections between sets, showing where events have common outcomes.
    - Non-overlapping regions represent the outcomes unique to each event.

    Venn diagrams are particularly useful for understanding the concepts of probability, including mutually exclusive events, independent events, and conditional probability.

2. Contingency Tables:

    - A contingency table, also known as a cross-tabulation or a two-way frequency table, is a tabular method used to show the distribution of two categorical variables and the frequency of their combinations.

    In a contingency table:

    - Rows represent one categorical variable.
    - Columns represent another categorical variable.
    - Cells in the table show the frequency or count of observations falling into each combination of the two variables.

    Contingency tables are widely used to analyze relationships and dependencies between categorical variables, especially in the context of conditional probability. They can help identify patterns, associations, and dependencies between variables.

## Joint Probability, Marginal Probability, Conditional Probability

1. Joint Probability:
    - Joint probability deals with the likelihood of two or more events happening together.
    - It's like asking, "What's the chance that both of these things occur at the same time?"
    - Imagine you're rolling a die twice, and you want to know the probability of getting a 3 on the first roll and a 5 on the second roll. That's an example of joint probability.

2. Marginal Probability:
    - Marginal probability focuses on the likelihood of a single event happening, without considering any other events.
    - It's like asking, "What's the chance of just this one thing happening?" Imagine you have a table showing the probability of having a certain hair color and a certain eye color.
    - If you're interested in the probability of having brown eyes regardless of hair color, you're looking at the marginal probability of eye color.

3. Conditional Probability:
    - Conditional probability involves the probability of one event happening given that another event has already happened.
    - It's like asking, "What's the chance of this thing happening, considering that we know this other thing has already occurred?"
    - Imagine you're picking a card from a deck, and you want to know the probability that it's a queen, given that it's a red card.

In simple terms:

- Joint probability is about both events happening at the same time.
- Marginal probability is about just one event happening.
- Conditional probability is about one event happening while considering another event that's already happened.

## Bayes' Theorem

- Bayes' theorem is a fundamental concept in probability theory that allows us to update the probability of an event based on new information.
- Bayes' theorem is particularly useful when dealing with conditional probabilities and making predictions or decisions using available data.

- The theorem can be expressed as follows:

    $$
    \\P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}\
    $$

  - P(A|B) is the posterior probability of event A occurring given that event B has occurred.
  - P(B|A) is the likelihood of event B occurring given that event A has occurred.
  - P(A) is the prior probability of event A occurring before considering any new evidence.
  - P(B) is the total probability of event B occurring.

- Bayes' theorem is commonly used to update beliefs or make predictions based on new data or observations. It's widely used in various fields, including statistics, machine learning, medical diagnosis, and information retrieval.
- The theorem forms the basis for understanding the relationships between conditional probabilities and helps us make informed decisions when new information becomes available.

- Let's walk through an example to illustrate how Bayes' theorem can be applied.
- Consider a medical scenario where we want to determine the probability that a patient has a certain disease given the results of a diagnostic test.

Example: Medical Diagnosis

Suppose there's a disease D and a diagnostic test T that can be used to detect the disease. Let's define the following probabilities:

- P(D): The prior probability that a randomly selected patient has the disease.
- P(T|D): The probability that the test is positive given that the patient has the disease (sensitivity).
- P(T|¬D): The probability that the test is positive given that the patient doesn't have the disease (false positive rate).
- We want to find P(D|T), the probability that a patient has the disease given that the test is positive.

Using Bayes' theorem:

$$
\\P(D|T) = \frac{P(T|D) \cdot P(D)}{P(T)}\
$$

- Here, P(T) is the total probability of testing positive, and it can be calculated using the law of total probability:

$$
\\P(T) = P(T|D) \cdot P(D) + P(T|\neg D) \cdot P(\neg D)\
$$

- Let's assume P(D) = 0.01 (1% of the population has the disease), P(T|D) = 0.95 (sensitivity of the test), and P(T|¬D) = 0.10 (false positive rate).

Calculating P(T):

$$
\\P(T) = P(T|D) \cdot P(D) + P(T|\neg D) \cdot P(\neg D)\
\\P(T) = 0.95 \cdot 0.01 + 0.10 \cdot 0.99 = 0.1045\
$$

Now we can use Bayes' theorem to find P(D|T):

$$
\\P(D|T) = \frac{P(T|D) \cdot P(D)}{P(T)}\
\\P(D|T) = \frac{0.95 \cdot 0.01}{0.1045} \approx 0.0909\
$$

- So, if a patient tests positive for the disease, the probability that they actually have the disease is approximately 9.09%.
- This demonstrates how Bayes' theorem can help us update our beliefs based on new evidence (in this case, the positive test result).
