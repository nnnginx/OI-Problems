## Description

<div><p><span class="tex-font-style-bf">This is the hard version of the problem. The difference between the versions is that in this version, the time limit and the constraints on $n$ and $q$ are higher. You can hack only if you solved all versions of this problem.</span> </p><p>Gellyfish has an array consisting of $n$ sets. Initially, all the sets are empty.</p><p>Now Gellyfish will do $q$ operations. Each operation contains one modification operation and one query operation, for the $i$-th ($1 \leq i \leq q$) operation:</p><p>First, there will be a modification operation, which is one of the following:</p><ol> <li> <span class="tex-font-style-bf">Insert</span> operation: You are given an integer $r$. For the $1$-th to $r$-th sets, insert element $i$. Note that the element inserted here is $i$, the index of the operation, not the index of the set. </li><li> <span class="tex-font-style-bf">Reverse</span> operation: You are given an integer $r$. Reverse the $1$-th to $r$-th sets. </li><li> <span class="tex-font-style-bf">Delete</span> operation: You are given an integer $x$. Delete element $x$ from all sets that contain $x$. </li></ol><p>Followed by a query operation:</p><ul> <li> <span class="tex-font-style-bf">Query</span> operation: You are given an integer $p$. Output the smallest element in the $p$-th set (If the $p$-th set is empty, the answer is considered to be $0$). </li></ul><p>Now, Flower needs to provide the answer for each query operation. Please help her!</p><p><span class="tex-font-style-bf">Additional constraint on the problem</span>: Gellyfish will only give the next operation after Flower has answered the previous query operation. That is, you need to solve this problem <span class="tex-font-style-bf">online</span>. Please refer to the input format for more details.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($1 \leq n, q \leq 3 \cdot 10^5$)&nbsp;！ the number of the sets and the number of operations.</p><p>As you need to respond to the operations online, the operations will be encoded.</p><p>The $i$-th line of the following $q$ lines contains three integers $a$, $b$, and $c$ ($1 \leq a \leq 3$, $1 \leq c \leq n$)&nbsp;！ describing the $i$-th operation in an encoded form.</p><p>Here, $a$ represents the type of modification operation. Among them, $a=1$ represents <span class="tex-font-style-bf">Insert</span> operation, $a=2$ represents <span class="tex-font-style-bf">Reverse</span> operation, $a=3$ represents <span class="tex-font-style-bf">Delete</span> operation.</p><ul> <li> If $a = 1$, then the modification operation is the <span class="tex-font-style-bf">Insert</span> operation. It will be guaranteed that $1 \leq b \leq n$. $r$ will be calculated as $r=(b+\text{ans}_{i-1}-1) \bmod n + 1$. </li><li> If $a=2$, then the modification operation is the <span class="tex-font-style-bf">Reverse</span> operation. It will be guaranteed that $1 \leq b \leq n$. $r$ will be calculated as $r=(b+\text{ans}_{i-1}-1) \bmod n + 1$. </li><li> If $a=3$, then the modification operation is the <span class="tex-font-style-bf">Delete</span> operation. It will be guaranteed that $1 \leq b \leq q$. $x$ will be calculated as $x=(b+\text{ans}_{i-1}-1) \bmod q + 1$. </li></ul><p>For the query operation, $p$ will be calculated as $p = (c+\text{ans}_{i-1}-1) \bmod n + 1$.</p><p>Here $ \text{ans}_{i} (1 \leq i \leq q)$ represents the answer to the query operation in the $i$-th operation. Additionally, we define $ \text{ans}_{0} = 0$.</p></div><div class="output-specification"><p>For each query operation, output the answer to the query.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($1 \leq n, q \leq 3 \cdot 10^5$)&nbsp;！ the number of the sets and the number of operations.</p><p>As you need to respond to the operations online, the operations will be encoded.</p><p>The $i$-th line of the following $q$ lines contains three integers $a$, $b$, and $c$ ($1 \leq a \leq 3$, $1 \leq c \leq n$)&nbsp;！ describing the $i$-th operation in an encoded form.</p><p>Here, $a$ represents the type of modification operation. Among them, $a=1$ represents <span class="tex-font-style-bf">Insert</span> operation, $a=2$ represents <span class="tex-font-style-bf">Reverse</span> operation, $a=3$ represents <span class="tex-font-style-bf">Delete</span> operation.</p><ul> <li> If $a = 1$, then the modification operation is the <span class="tex-font-style-bf">Insert</span> operation. It will be guaranteed that $1 \leq b \leq n$. $r$ will be calculated as $r=(b+\text{ans}_{i-1}-1) \bmod n + 1$. </li><li> If $a=2$, then the modification operation is the <span class="tex-font-style-bf">Reverse</span> operation. It will be guaranteed that $1 \leq b \leq n$. $r$ will be calculated as $r=(b+\text{ans}_{i-1}-1) \bmod n + 1$. </li><li> If $a=3$, then the modification operation is the <span class="tex-font-style-bf">Delete</span> operation. It will be guaranteed that $1 \leq b \leq q$. $x$ will be calculated as $x=(b+\text{ans}_{i-1}-1) \bmod q + 1$. </li></ul><p>For the query operation, $p$ will be calculated as $p = (c+\text{ans}_{i-1}-1) \bmod n + 1$.</p><p>Here $ \text{ans}_{i} (1 \leq i \leq q)$ represents the answer to the query operation in the $i$-th operation. Additionally, we define $ \text{ans}_{0} = 0$.</p>

## Output

<p>For each query operation, output the answer to the query.</p>





```input1|
5 10
1 2 2
2 3 1
1 5 3
2 2 5
1 5 2
2 4 4
3 2 2
3 1 2
3 10 5
3 2 4
```




```output1
1
0
1
1
3
1
0
5
0
0
```



## Note

<p>All the sets are empty in the beginning, so the array is $[\{\}, \{\}, \{\}, \{\}, \{\}]$.</p><p>With the decoding method given before, we can see what happens in each operation:</p><ol> <li> For the first operation: $a = 1, r = 2, p = 2$. The modification operation is an <span class="tex-font-style-bf">Insert</span> operation; element $1$ is inserted into the first two sets; so the array becomes $[\{1\}, \{1\}, \{\}, \{\}, \{\}]$, and the smallest element in the second set is $1$.</li><li> For the second operation: $a = 2, r = 4, p = 2$. The modification operation is a <span class="tex-font-style-bf">Reverse</span> operation; the first four sets are reversed; so the array becomes $[\{\}, \{\}, \{1\}, \{1\}, \{\}]$, and the second set is empty, which means the answer is $0$.</li><li> For the third operation: $a = 1, r = 5, p = 3$. The modification operation is an <span class="tex-font-style-bf">Insert</span> operation; element $3$ is inserted into all the sets; so the array becomes $[\{3\}, \{3\}, \{1, 3\}, \{1, 3\}, \{3\}]$, and the smallest element in the third set is $1$.</li><li> For the fourth operation: $a = 2, r = 3, p = 1$. The modification operation is a <span class="tex-font-style-bf">Reverse</span> operation; the first three sets are reversed; so the array becomes $[\{1, 3\}, \{3\}, \{3\}, \{1, 3\}, \{3\}]$, and the smallest element in the first set is $1$.</li><li> For the fifth operation: $a = 1, r = 1, p = 3$. The modification operation is an <span class="tex-font-style-bf">Insert</span> operation; element $5$ is inserted into the first set; so the array becomes $[\{1, 3, 5\}, \{3\}, \{3\}, \{1, 3\}, \{3\}]$, and the smallest element in the third set is $3$.</li><li> For the sixth operation: $a = 2, r = 2, p = 2$. The modification operation is a <span class="tex-font-style-bf">Reverse</span> operation; the first two sets are reversed; so the array becomes $[\{3\}, \{1, 3, 5\}, \{3\}, \{1, 3\}, \{3\}]$, and the smallest element in the second set is $1$.</li><li> For the seventh operation: $a = 3, x = 3, p = 3$. The modification operation is a <span class="tex-font-style-bf">Delete</span> operation; element $3$ is deleted from all the sets; so the array becomes $[\{\}, \{1, 5\}, \{\}, \{1\}, \{\}]$, and the third set is empty, which means the answer is $0$.</li><li> For the eighth operation: $a = 3, x = 1, p = 2$. The modification operation is a <span class="tex-font-style-bf">Delete</span> operation; element $1$ is deleted from all the sets; so the array becomes $[\{\}, \{5\}, \{\}, \{\}, \{\}]$, and the smallest element in the second set is $5$.</li><li> For the ninth operation: $a = 3, x = 5, p = 5$. The modification operation is a <span class="tex-font-style-bf">Delete</span> operation; element $5$ is deleted from all the sets; so the array becomes $[\{\}, \{\}, \{\}, \{\}, \{\}]$, and the fifth set is empty, which means the answer is $0$.</li><li> For the tenth operation: $a = 3, x = 2, p = 4$. The modification operation is a <span class="tex-font-style-bf">Delete</span> operation; element $2$ is deleted from all the sets; so the array becomes $[\{\}, \{\}, \{\}, \{\}, \{\}]$, and the fourth set is empty, which means the answer is $0$. </li></ol><p>Please note that although we have not inserted element $2$ into the sets, we still delete element $2$ from all the sets in the tenth operation, which means that the <span class="tex-font-style-bf">Delete</span> operation doesn't necessarily require the existence of a set to contain the deleted element. It also shows that it is possible to have two <span class="tex-font-style-bf">Delete</span> operations that delete the same element.</p>
