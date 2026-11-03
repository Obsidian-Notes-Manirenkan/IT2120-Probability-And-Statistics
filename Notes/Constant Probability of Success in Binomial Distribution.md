In a binomial distribution, the same simple experiment is repeated several times. Each attempt is called a **trial**, and each trial ends in either a **success** or a **failure**.

Saying that the probability of success, $p$, is **constant** means that it is the same number in every trial. It does not go up or down from one trial to the next, no matter what happened before.

---
## Example: Tossing a Fair Coin

Let "success" mean getting a head, so $p = 0.5$.

- 1st toss: $p = 0.5$
- 2nd toss: $p = 0.5$, even if the 1st toss was a head
- 10th toss: $p = 0.5$, even after nine heads in a row

The coin does not remember what happened before, so the probability never changes.

---

## A Case Where It Does Not Hold

A bag has 3 red balls and 2 blue balls. A ball is picked and kept out, then a second ball is picked. "Success" means getting a red ball.

$$
P(\text{red on 1st pick}) = \frac{3}{5}
$$

If the first ball was red, then:

$$
P(\text{red on 2nd pick}) = \frac{2}{4}
$$

The probability changed because the contents of the bag changed, so this is **not** a binomial situation. It becomes binomial if the ball is **replaced** after each pick, because then $p = \frac{3}{5}$ every time.

---

## Why It Matters

The binomial formula assumes one fixed $p$ and uses it in every trial:

$$
P(X = x) = \binom{n}{x}\,p^{x}(1-p)^{n-x}
$$

If $p$ kept changing, the probability could not be written using a single $p$, and this formula would give wrong answers.

---

## Conditions for a Binomial Setting

- A fixed number of trials, $n$.
- Each trial has only two outcomes, success or failure.
- The trials are **independent**, so one result does not affect another.
- The probability of success, $p$, is **constant** for every trial.
