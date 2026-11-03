A **random variable** is a variable whose value is a **number determined by the outcome of a random experiment**.

In other words, it takes something that happens by chance and turns it into a number that can be worked with.

Formally, a random variable is a function that maps each outcome in the sample space $S$ to a real number:

$$
X : S \rightarrow \mathbb{R}
$$

![[Pasted image 20261102112105.png]]

---

## Example

Toss a coin twice. The outcomes are HH, HT, TH, and TT, which are not numbers. Define $X$ as the number of heads.

| Outcome | HH | HT | TH | TT |
|---|---|---|---|---|
| $X$ | $2$ | $1$ | $1$ | $0$ |

$X$ is a random variable. Before the coins are tossed, the value of $X$ is unknown, but the values it could take ($0$, $1$, or $2$) and how likely each one is are known.

The probability of each value is:

$$
P(X=0)=\frac{1}{4}, \qquad P(X=1)=\frac{1}{2}, \qquad P(X=2)=\frac{1}{4}
$$

---

## Types of Random Variables

- **Discrete:** takes countable values, such as the number of heads, the number of defective items, or the number of customers in an hour.
- **Continuous:** takes any value in an interval, such as height, time, or temperature.

---

## Notation

- A capital letter, such as $X$, is the random variable itself.
- A small letter, such as $x$, is a particular value that the random variable takes.
- $P(X = x)$ is the probability that $X$ equals $x$.

A random variable lets us use mathematics, such as probabilities, means, and variances, on random situations.

---

[[Cumulative Distribution Function]]
[[Constant Probability of Success in Binomial Distribution]]