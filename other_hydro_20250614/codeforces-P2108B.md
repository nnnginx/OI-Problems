## Description

<div><p> </p><p>On a recent birthday, your best friend Maurice gave you a pair of numbers $n$ and $x$, and asked you to construct an array of <span class="tex-font-style-bf">positive</span> numbers $a$ of length $n$ such that $a_1 \oplus a_2 \oplus \cdots \oplus a_n = x$ $^{\text{∗}}$. </p><p>This task seemed too simple to you, and therefore you decided to give Maurice a return gift by constructing an array among all such arrays that has the smallest sum of its elements. You immediately thought of a suitable array; however, since writing it down turned out to be too time-consuming, Maurice will have to settle for just the sum of its elements.</p><div class="statement-footnote"><p>$^{\text{∗}}$$\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>. </p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>Each test case consists of a single line containing a pair of numbers $n$ and $x$ ($1 \le n \le 10^9, \; 0 \le x \le 10^9$)&nbsp;— the numbers given to you by Maurice.</p></div><div class="output-specification"><p>For each test case, output your gift to Maurice&nbsp;— the sum of the elements of the array that satisfies all the described properties. If a suitable array does not exist, output $-1$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>Each test case consists of a single line containing a pair of numbers $n$ and $x$ ($1 \le n \le 10^9, \; 0 \le x \le 10^9$)&nbsp;— the numbers given to you by Maurice.</p>

## Output

<p>For each test case, output your gift to Maurice&nbsp;— the sum of the elements of the array that satisfies all the described properties. If a suitable array does not exist, output $-1$.</p>





```input1|2,4,6,8
8
2 1
3 6
1 0
2 0
5 0
2 27
15 43
12345678 9101112
```




```output1
5
8
-1
2
8
27
55
21446778
```



## Note

<p>In the first test case, one of the suitable arrays is $[2, 3]$. It can be shown that it is impossible to achieve a smaller sum of array elements.</p><p>In the second case, one of the suitable arrays is $[1, 3, 4]$. It can also be shown that this is the optimal amount.</p>
