The **cumulative distribution function (c.d.f.)** of a random variable $X$ is defined by:

$$
F_X(x) = P(X \leq x)
$$

---

## Meaning

- $F_X(x)$ is the probability that $X$ takes a value **less than or equal to** $x$.
- It is a running total: it accumulates the probability of everything up to and including $x$.
- Any real number $x$ can be used as the input, not only the values that $X$ can take.
- The subscript $X$ states which random variable the function belongs to. The input $x$ is just a number that is chosen.

---

## Discrete Example

Let $X$ be the number of heads in two coin tosses, with:

$$
P(X=0)=\frac{1}{4}, \qquad P(X=1)=\frac{1}{2}, \qquad P(X=2)=\frac{1}{4}
$$

Add up the probabilities up to each value.

$$
F_X(0) = P(X \leq 0) = \frac{1}{4}
$$

$$
F_X(1) = P(X \leq 1) = \frac{1}{4} + \frac{1}{2} = \frac{3}{4}
$$

$$
F_X(2) = P(X \leq 2) = \frac{1}{4} + \frac{1}{2} + \frac{1}{4} = 1
$$

For values between these points, the c.d.f. stays flat. For example:

$$
F_X(1.5) = P(X \leq 1.5) = P(X \leq 1) = \frac{3}{4}
$$

The full function is:

$$
F_X(x) =
\begin{cases}
0, & x < 0 \\
\frac{1}{4}, & 0 \leq x < 1 \\
\frac{3}{4}, & 1 \leq x < 2 \\
1, & x \geq 2
\end{cases}
$$

This is a **step function**. It jumps at each value that $X$ can take, and the size of each jump equals the probability at that value.

---

## Continuous Case

If $X$ is continuous with probability density function $f(x)$, the c.d.f. is the area under the curve up to $x$:

$$
F_X(x) = \int_{-\infty}^{x} f(t)\,dt
$$

Going the other way, the density is the derivative of the c.d.f. (where it exists):

$$
f(x) = \frac{d}{dx}F_X(x)
$$

---

## Key Properties

- **Non-decreasing:** if $a < b$, then $F_X(a) \leq F_X(b)$, because including more values can only add probability.
- **Limits:** $F_X(x) \to 0$ as $x \to -\infty$ and $F_X(x) \to 1$ as $x \to \infty$.
- **Bounded:** $0 \leq F_X(x) \leq 1$ for all $x$.
- **Right-continuous:** there are no gaps on the "less than or equal to" side of each jump.

---

## Uses

The c.d.f. gives the probability of an interval directly:

$$
P(a < X \leq b) = F_X(b) - F_X(a)
$$

Using the coin example:

$$
P(0 < X \leq 2) = F_X(2) - F_X(0) = 1 - \frac{1}{4} = \frac{3}{4}
$$

It also gives "greater than" probabilities through the complement:

$$
P(X > a) = 1 - F_X(a)
$$
