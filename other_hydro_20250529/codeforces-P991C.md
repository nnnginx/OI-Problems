## Description

<div><p>After passing a test, Vasya got himself a box of $n$ candies. He decided to eat an equal amount of candies each morning until there are no more candies. However, Petya also noticed the box and decided to get some candies for himself.</p><p>This means the process of eating candies is the following: in the beginning Vasya chooses a single integer $k$, same for all days. After that, in the morning he eats $k$ candies from the box (if there are less than $k$ candies in the box, he eats them all), then in the evening Petya eats $10\%$ of the candies <span class="tex-font-style-bf">remaining</span> in the box. If there are still candies left in the box, the process repeats&nbsp;！ next day Vasya eats $k$ candies again, and Petya&nbsp;！ $10\%$ of the candies left in a box, and so on.</p><p>If the amount of candies in the box is not divisible by $10$, Petya rounds the amount he takes from the box down. For example, if there were $97$ candies in the box, Petya would eat only $9$ of them. In particular, if there are less than $10$ candies in a box, Petya won't eat any at all.</p><p>Your task is to find out the minimal amount of $k$ that can be chosen by Vasya so that he would eat at least half of the $n$ candies he initially got. Note that the number $k$ must be integer.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 10^{18}$)&nbsp;！ the initial amount of candies in the box.</p></div><div class="output-specification"><p>Output a single integer&nbsp;！ the minimal amount of $k$ that would allow Vasya to eat at least half of candies he got.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 10^{18}$)&nbsp;！ the initial amount of candies in the box.</p>

## Output

<p>Output a single integer&nbsp;！ the minimal amount of $k$ that would allow Vasya to eat at least half of candies he got.</p>

## Samples

```input1
68

```

```output1
3

```




## Note

<p>In the sample, the amount of candies, with $k=3$, would change in the following way (Vasya eats first):</p><p>$68 \to 65 \to 59 \to 56 \to 51 \to 48 \to 44 \to 41 \\ \to 37 \to 34 \to 31 \to 28 \to 26 \to 23 \to 21 \to 18 \to 17 \to 14 \\ \to 13 \to 10 \to 9 \to 6 \to 6 \to 3 \to 3 \to 0$.</p><p>In total, Vasya would eat $39$ candies, while Petya&nbsp;！ $29$.</p>
