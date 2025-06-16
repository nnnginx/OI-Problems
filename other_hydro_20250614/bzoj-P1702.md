## 题目描述
Farmer John's $n$ cows $(1 \le n \le 10^5)$ share many similarities. In fact, FJ has been able to narrow down the list of features shared by his cows to a list of only $k$ different features $(1 \le k \le 30)$. For example, cows exhibiting feature #1 might have spots, cows exhibiting feature #2 might prefer C to Pascal, and so on. FJ has even devised a concise way to describe each cow in terms of its "feature ID", a single k-bit integer whose binary representation tells us the set of features exhibited by the cow. As an example, suppose a cow has feature ID = $13$. Since $13$ written in binary is $1101$, this means our cow exhibits features $1$, $3$, and $4$ (reading right to left), but not feature $2$. More generally, we find a $1$ in the $2^{i-1}$ place if a cow exhibits feature $i$. Always the sensitive fellow, FJ lined up cows $1\dots n$ in a long row and noticed that certain ranges of cows are somewhat "balanced" in terms of the features the exhibit. A contiguous range of cows $i\dots j$ is balanced if each of the $k$ possible features is exhibited by the same number of cows in the range. FJ is curious as to the size of the largest balanced range of cows. See if you can determine it.

$n$ 头牛，一共 $k$ 种特色，每头牛有多种特色，用二进制 $01$ 表示它的特色 ID。比如特色 ID 为 $13(1101)$，则它有第 $1$、$3$、$4$ 种特色。$[i,j]$ 段被称为 balanced 当且仅当 $k$ 种特色在 $[i,j]$ 内拥有次数相同。求最大的 $[i,j]$ 段长度。
## 输入格式
* Line $1$: Two space-separated integers, $n$ and $k$.
* Lines $2\dots n+1$: Line $i+1$ contains a single $k$-bit integer specifying the features present in cow $i$. The least-significant bit of this integer is $1$ if the cow exhibits feature #1, and the most-significant bit is $1$ if the cow exhibits feature #k.
## 输出格式
* Line $1$: A single integer giving the size of the largest contiguous balanced group of cows.

```input1
7 3
7
6
7
2
1
4
2
```
```output1
4
```
## 样例说明
INPUT DETAILS:  
The line has $7$ cows with $3$ features; the table below summarizes the correspondence:

|Feature $3$:|$1$|$1$|$1$|$0$|$0$|$1$|$0$|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|Feature $2$:| $1$|$1$ |$1$|$1$|$0$|$0$|$1$|
|Feature $1$:|$1$ |$0$|$1$|$0$|$1$|$0$|$0$|
|key:|$7$|$6$|$7$|$2$|$1$|$4$|$2$|
|Cow #:|$1$|$2$|$3$|$4$|$5$|$6$|$7$|

OUTPUT DETAILS:  
In the range from cow #3 to cow #6 (of size $4$), each feature appears in exactly $2$ cows in this range:

|Feature $3$:|$1$|$0$|$0$|$1$|-> two total|
| :--------: | :--: | :--: | :--: | :--: | :--: |
|Feature $2$:| $1$|$1$ |$0$| $0$|-> two total|
|Feature $1$:|$1$|$0$|$1$|$0$ |-> two total|
|key:|$7$|$2$|$1$ |$4$| |
|Cow #:|$3$|$4$|$5$|$6$| |
## 数据规模与约定
对于 $100\%$ 的数据，$1\le n\le10^5$，$1\le k\le30$。
## 题目来源
鸣谢[fjxmyzwd](http://61.187.179.132/JudgeOnline/userinfo.php?user=fjxmyzwd)

Gold