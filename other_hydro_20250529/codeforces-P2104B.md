## Description

<div><p>You are given an array $a$ consisting of $n$ integers.</p><p>For every integer $k$ from $1$ to $n$, you have to do the following:</p><ol> <li> choose an arbitrary element of $a$ and move it to the right end of the array (you can choose the last element, then the array won't change); </li><li> print the sum of $k$ last elements of $a$; </li><li> move the element you've chosen on the first step to its original position (restore the original array $a$). </li></ol><p>For every $k$, you choose the element which you move so that the value you print is <span class="tex-font-style-bf">the maximum possible</span>.</p><p>Calculate the value you print for every $k$.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \le t \le 10^4$) ¡ª the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$); </li><li> the second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$). </li></ul><p>Additional constraint on the input: the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, print $n$ integers. The $i$-th of these integers should be equal to the maximum value you can print if $k=i$.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \le t \le 10^4$) ¡ª the number of test cases.</p><p>Each test case consists of two lines:</p><ul> <li> the first line contains one integer $n$ ($1 \le n \le 2 \cdot 10^5$); </li><li> the second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$). </li></ul><p>Additional constraint on the input: the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, print $n$ integers. The $i$-th of these integers should be equal to the maximum value you can print if $k=i$.</p>





```input1|2,3,6,7
4
7
13 5 10 14 8 15 13
6
1000000000 1000000000 1000000000 1000000000 1000000000 1000000000
1
42
2
7 5
```




```output1
15 28 42 50 63 73 78 
1000000000 2000000000 3000000000 4000000000 5000000000 6000000000 
42 
7 12
```



## Note

<p>Let's consider the first test case from the statement:</p><ul> <li> when $k = 1$, you can move the $6$-th element to the end, the array becomes $[13, 5, 10, 14, 8, 13, 15]$, and the value you print is $15$; </li><li> when $k = 2$, you can move the $6$-th element to the end, the array becomes $[13, 5, 10, 14, 8, 13, 15]$, and the value you print is $13 + 15 = 28$; </li><li> when $k = 3$, you can move the $4$-th element to the end, the array becomes $[13, 5, 10, 8, 15, 13, 14]$, and the value you print is $15 + 13 + 14 = 42$; </li><li> when $k = 4$, you can move the $5$-th element to the end, the array becomes $[13, 5, 10, 14, 15, 13, 8]$, and the value you print is $14 + 15 + 13 + 8 = 50$; </li><li> when $k = 5$, you can move the $1$-st element to the end, the array becomes $[5, 10, 14, 8, 15, 13, 13]$, and the value you print is $14 + 8 + 15 + 13 + 13 = 63$; </li><li> when $k = 6$, you can move the $1$-st element to the end, the array becomes $[5, 10, 14, 8, 15, 13, 13]$, and the value you print is $10 + 14 + 8 + 15 + 13 + 13 = 73$; </li><li> when $k = 7$, you can move the $6$-th element to the end, the array becomes $[13, 5, 10, 14, 8, 13, 15]$, and the value you print is $13 + 5 + 10 + 14 + 8 + 13 + 15 = 78$. </li></ul>
