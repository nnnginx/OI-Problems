## 题目描述
  
Evolution is a seemingly random process which works in a way which resembles certain approaches we use to get approximate solutions to hard combinatorial problems．You are now to do something completely different．  
Given a DNA string $S$ from the alphabet $\text{A,C,G,T}$，find the minimal number of copy operations needed to create another string $T$．You may reverse the strings you copy，and copy both from $S$ and the pieces of your partial $T$．You may put these pieces together at any time．You may only copy contiguous parts of your partial $T$，and all copied strings must be used in your final $T$．

```
Example：From S={ACTG} create T={GTACTATTATA}
Get GT......... by copying and reversing 「TG」 from S．
Get GTAC....... by copying 「AC」 from S．
Get GTAC...TA.. by copying 「TA」 from the partial T．
Get GTAC...TAAT by copying and reversing 「TA」 from the partial T．
Get GTACAATTAAT by copying 「AAT」 from the partial T．
```

给你两个字符串 $S$ 和 $T$，要求你用尽量少的步数从 $S$ 构造出 $T$。每一步你可以做以下操作：从 $S$ 或者 $T$ 的片段中拷贝一个字符串，然后可以将这个字符串反向，然后你得到一个片段。片段可以随时合并，但不能拆分，并且所有的片段都要使用。从 $T$ 中拷贝字符串只能从一个片段中拷贝。求你最少需要的步数。两个串的字符数 $\le 18$。

## 输入格式

The first line of input gives a single integer，t，the number of test cases．  
Then follow，for each test case，a line with the string $S$ of length $m$ and a line with the string $T$ of length $n$．

## 输出格式

Output for each test case the number of copy operations needed to create $T$ from $S$，or `impossible` if it cannot be done．

```input1
5
ACGT
GTAC
A
C
ACGT
TGCA
ACGT
TCGATCGA
A
AAAAAAAAAAAAAAAAAA
```

```output1
2
impossible
1
4
6
```

## 数据规模与约定

$100\%$ 的数据满足：$1 \le t \le 100$，$1 \le m,n \le 18$。

