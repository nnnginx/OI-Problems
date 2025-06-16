## Description

<div><p>Hackers are once again trying to create entertaining phrases using the output of neural networks. This time, they want to obtain an array of strings $a$ of length $n$.</p><p>Initially, they have an array $c$ of length $n$, filled with blanks, which are denoted by the symbol $*$. Thus, if $n=4$, then initially $c=[*,*,*,*]$.</p><p>The hackers have access to $m$ neural networks, each of which has its own version of the answer to their request – an array of strings $b_i$ of length $n$.</p><p>The hackers are trying to obtain the array $a$ from the array $c$ using the following operations: </p><ol> <li> Choose a neural network $i$, which will perform the next operation on the array $c$: it will select a <span class="tex-font-style-it"><span class="tex-font-style-bf">random</span></span> <span class="tex-font-style-bf">blank</span>, for example, at position $j$, and replace $c_j$ with $b_{i, j}$.<p>For example, if the first neural network is chosen and $c = [*, \text{«like»}, *]$, and $b_1 = [\text{«I»}, \text{«love»}, \text{«apples»}]$, then after the operation with the first neural network, $c$ may become either $[\text{«I»}, \text{«like»}, *]$ or $[*, \text{«like»}, \text{«apples»}]$.</p></li><li> Choose position $j$ and replace $c_j$ with a blank. </li></ol><p>Unfortunately, because of the way hackers access neural networks, they will only be able to see the modified array $c$ after all operations are completed, so they will have to specify the entire sequence of operations in advance.</p><p>However, the random behavior of the neural networks may lead to the situation where the desired array is never obtained, or obtaining it requires an excessive number of operations. </p><p>Therefore, the hackers are counting on your help in choosing a sequence of operations that will guarantee the acquisition of array $a$ in the minimum number of operations.</p><p>More formally, if there exists a sequence of operations that can <span class="tex-font-style-bf">guarantee</span> obtaining array $a$ from array $c$, then among all such sequences, find the one with the <span class="tex-font-style-bf">minimum</span> number of operations, and output the number of operations in it.</p><p>If there is no sequence of operations that transforms array $c$ into array $a$, then output $-1$.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 500$)&nbsp;— the length of the original array $a$ and the number of neural networks, respectively.</p><p>The second line of each test case contains the array $a$, consisting of $n$ strings $a_i$ ($1 \le |a_i| \le 10$), separated by spaces.</p><p>The next $m$ lines of each test case contain the arrays $b_i$&nbsp;— one in each line, consisting of $n$ strings $b_{i, j}$ ($1 \le |b_{i,j}| \le 10$), separated by spaces.</p><p>It is guaranteed that the sum of $|a_i|$ and $|b_{i, j}|$ across all test cases does not exceed $2 \cdot 10^5$, and that the sum of $n \cdot m$ across all test cases also does not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that the input strings consist only of characters from the Latin alphabet in both lowercase and uppercase.</p><p>Note that the length of each individual input string does not exceed $10$.</p></div><div class="output-specification"><p>Output $t$ numbers&nbsp;— one number for each test case, each on a separate line.</p><p>If there exists a sequence of operations that guarantees obtaining array $a$ from the $i$-th test case, then the $i$-th number is the number of operations in the minimum such sequence.</p><p>Otherwise, for the $i$-th number, output $-1$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \le n, m \le 500$)&nbsp;— the length of the original array $a$ and the number of neural networks, respectively.</p><p>The second line of each test case contains the array $a$, consisting of $n$ strings $a_i$ ($1 \le |a_i| \le 10$), separated by spaces.</p><p>The next $m$ lines of each test case contain the arrays $b_i$&nbsp;— one in each line, consisting of $n$ strings $b_{i, j}$ ($1 \le |b_{i,j}| \le 10$), separated by spaces.</p><p>It is guaranteed that the sum of $|a_i|$ and $|b_{i, j}|$ across all test cases does not exceed $2 \cdot 10^5$, and that the sum of $n \cdot m$ across all test cases also does not exceed $2 \cdot 10^5$.</p><p>It is guaranteed that the input strings consist only of characters from the Latin alphabet in both lowercase and uppercase.</p><p>Note that the length of each individual input string does not exceed $10$.</p>

## Output

<p>Output $t$ numbers&nbsp;— one number for each test case, each on a separate line.</p><p>If there exists a sequence of operations that guarantees obtaining array $a$ from the $i$-th test case, then the $i$-th number is the number of operations in the minimum such sequence.</p><p>Otherwise, for the $i$-th number, output $-1$.</p>





```input1
4
3 3
I love apples
He likes apples
I love cats
They love dogs
3 2
Icy wake up
wake Icy up
wake up Icy
4 3
c o D E
c o D s
c O l S
c o m E
4 5
a s k A
d s D t
O R i A
a X b Y
b a k A
u s k J
```




```output1
5
-1
6
8
```


