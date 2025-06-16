## Description

<div><p>Burenka came to kindergarden. This kindergarten is quite strange, so each kid there receives two fractions ($\frac{a}{b}$ and $\frac{c}{d}$) with integer numerators and denominators. Then children are commanded to play with their fractions.</p><p>Burenka is a clever kid, so she noticed that when she claps once, she can multiply numerator or denominator of one of her two fractions by any integer of her choice (but she can't multiply denominators by $0$). Now she wants know the minimal number of claps to make her fractions equal (by <span class="tex-font-style-bf">value</span>). Please help her and find the required number of claps!</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$) �� the number of test cases. Then follow the descriptions of each test case.</p><p>The only line of each test case contains four integers $a$, $b$, $c$ and $d$ ($0 \leq a, c \leq 10^9$, $1 \leq b, d \leq 10^9$) �� numerators and denominators of the fractions given to Burenka initially.</p></div><div class="output-specification"><p>For each test case print a single integer �� the minimal number of claps Burenka needs to make her fractions equal.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^4$) �� the number of test cases. Then follow the descriptions of each test case.</p><p>The only line of each test case contains four integers $a$, $b$, $c$ and $d$ ($0 \leq a, c \leq 10^9$, $1 \leq b, d \leq 10^9$) �� numerators and denominators of the fractions given to Burenka initially.</p>

## Output

<p>For each test case print a single integer �� the minimal number of claps Burenka needs to make her fractions equal.</p>

## Samples

```input1
<div class="test-example-line test-example-line-even test-example-line-0">8</div><div class="test-example-line test-example-line-odd test-example-line-1">2 1 1 1</div><div class="test-example-line test-example-line-even test-example-line-2">6 3 2 1</div><div class="test-example-line test-example-line-odd test-example-line-3">1 2 2 3</div><div class="test-example-line test-example-line-even test-example-line-4">0 1 0 100</div><div class="test-example-line test-example-line-odd test-example-line-5">0 1 228 179</div><div class="test-example-line test-example-line-even test-example-line-6">100 3 25 6</div><div class="test-example-line test-example-line-odd test-example-line-7">999999999 300000000 666666666 100000000</div><div class="test-example-line test-example-line-even test-example-line-8">33 15 0 84</div><div class="test-example-line test-example-line-even test-example-line-8"></div>
```

```output1
1
0
2
0
1
1
1
1
```




## Note

<p>In the first case, Burenka can multiply $c$ by $2$, then the fractions will be equal.</p><p>In the second case, fractions are already equal.</p><p>In the third case, Burenka can multiply $a$ by $4$, then $b$ by $3$. Then the fractions will be equal ($\frac{1 \cdot 4}{2 \cdot 3} = \frac{2}{3}$).</p>
