## 题目描述
The famous polymath Nicolaus Copernicus was born and grew up in Toruń in the 15th century. Archaeologists have recently discovered his notebook, and learned that he was fond of using powers of two to store large numbers. In particular, even when he added two powers of two:

$$2^a + 2^b$$

Copernicus evaluated the result and then rounded up the result to the nearest power of two. That is, he would evaluate $2^a + 2^b$ to $2^{\max(a,b)+1}$. To evaluate a longer expression of the form:

$$2^{b_1}+2^{b_2}+\cdots + 2^{b_r}$$

he first inserted the brackets to make it well - parenthesised*. For example, an expression $2^5 + 2^4+2^4 + 2^4+2^5$ can be made well - parenthesised to obtain $((2^5 + 2^4)+(2^4+(2^4 + 2^5)))$. Finally, he evaluated the result of the obtained well - parenthesised expression, operating on powers of two as described above. Notice that the result might vary depending on how he inserts the brackets. For example, here are two possible ways to evaluate $2^5 + 2^4+2^4 + 2^4+2^5$:

$((2^5 + 2^4)+(2^4 + 2^5))=((2^6+2^4)+2^5)=(2^7 + 2^6)=2^8$

$((2^5+(2^4 + 2^4))+(2^4 + 2^5))=((2^5 + 2^5)+2^6)=(2^6+2^6)=2^7$

The first page of the Copernicus' notebook contains only a single expression $2^{a_1}+2^{a_2}+\cdots + 2^{a_n}$ called the main expression. Later pages of the notebook then reference fragments of the main expression, which are of the form $2^{a_\ell}+2^{a_{\ell + 1}}+\cdots + 2^{a_r}$, for some $1\leq \ell\leq r\leq n$.

You are not sure what their meaning, but suspect that you should calculate, for each such fragment, the smallest possible result that can be obtained when evaluating the result as described above for the fragment. Note that each fragment is evaluated independently of the other fragments.

## 输入格式
The first line contains two integers $n$ and $q$ ($1\leq n,q\leq300000$) denoting the length of the main expression from the first page of the notebook and the number of queries, respectively.

The second line contains $n$ integers $a_1,a_2,\cdots,a_n$ ($0\leq a_i\leq 10^9$), where the $i$ - th integer $a_i$ denotes the exponent of the $i$ - th power of two in the main expression.

The next $q$ lines describe the queries. Each query consists of two integers $\ell$ and $r$ ($1\leq \ell\leq r\leq n$) representing a fragment of the main expression starting at the $\ell$ - th power of two and ending at the $r$ - th power of two.

## 输出格式
You should output $q$ lines. The $i$ - th line should contain the smallest possible result that can be obtained when evaluating the fragment described in the $i$ - th query. You should output only the exponent of the corresponding power of two.

```input1
8 4
2 4 2 5 4 4 4 5
4 8
1 4
2 5
1 7
```

```output1
7
7
7
8
```

## 提示
| Subtasks | Constrains | Score |
| :---: | :---: | :---: |
| 1 | $n \leq 8, q \leq 10$ | 6 |
| 2 | $n \leq 200$ | 8 |
| 3 | $n, q \leq 2000$ | 23 |
| 4 | $a_{i} \leq 20$ | 22 |
| 5 | No addition constrains | 41 |

