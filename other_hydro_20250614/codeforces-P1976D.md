## Description

<div><p>A regular bracket sequence is a bracket sequence that can be transformed into a correct arithmetic expression by inserting characters '<span class="tex-font-style-tt">1</span>' and '<span class="tex-font-style-tt">+</span>' between the original characters of the sequence. For example:</p><ul> <li> bracket sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">(())</span>" are regular (the resulting expressions are: "<span class="tex-font-style-tt">(1)+(1)</span>" and "<span class="tex-font-style-tt">((1+1)+1)</span>"); </li><li> bracket sequences "<span class="tex-font-style-tt">)(</span>", "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" are not. </li></ul><p>Let's define the <span class="tex-font-style-it">inverse</span> of the bracket sequence as follows: replace all brackets '<span class="tex-font-style-tt">(</span>' with '<span class="tex-font-style-tt">)</span>', and vice versa (all brackets '<span class="tex-font-style-tt">)</span>' with '<span class="tex-font-style-tt">(</span>'). For example, strings "<span class="tex-font-style-tt">()((</span>" and "<span class="tex-font-style-tt">)())</span>" are inverses of each other.</p><p>You are given a regular bracket sequence $s$. Calculate the number of pairs of integers $(l,r)$ ($1 \le l \le r \le |s|$) such that if you replace the substring of $s$ from the $l$-th character to the $r$-th character (inclusive) with its inverse, $s$ will still be a regular bracket sequence.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a non-empty regular bracket sequence; it consists only of characters '<span class="tex-font-style-tt">(</span>' and/or '<span class="tex-font-style-tt">)</span>'.</p><p>Additional constraint on the input: the total length of the regular bracket sequences over all test cases doesn't exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the number of pairs $(l,r)$ meeting the conditions from the statement.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The only line of each test case contains a non-empty regular bracket sequence; it consists only of characters '<span class="tex-font-style-tt">(</span>' and/or '<span class="tex-font-style-tt">)</span>'.</p><p>Additional constraint on the input: the total length of the regular bracket sequences over all test cases doesn't exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print a single integer&nbsp;！ the number of pairs $(l,r)$ meeting the conditions from the statement.</p>





```input1|2,4
4
(())
()
()()()
(()())(())
```




```output1
1
0
3
13
```



## Note

<p>In the first example, there is only one pair: </p><ul> <li> $(2, 3)$: <span class="tex-font-style-tt">(())</span> $\rightarrow$ <span class="tex-font-style-tt">()()</span>. </li></ul><p>In the second example, there are no pairs.</p><p>In the third example, there are three pairs: </p><ul> <li> $(2, 3)$: <span class="tex-font-style-tt">()()()</span> $\rightarrow$ <span class="tex-font-style-tt">(())()</span>; </li><li> $(4, 5)$: <span class="tex-font-style-tt">()()()</span> $\rightarrow$ <span class="tex-font-style-tt">()(())</span>; </li><li> $(2, 5)$: <span class="tex-font-style-tt">()()()</span> $\rightarrow$ <span class="tex-font-style-tt">(()())</span>; </li></ul>
