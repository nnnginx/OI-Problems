## 题目描述
给出三个整数 $a,b,c$，保证 $b \neq 0$。

- 如果 $a + b = c$，请你输出 $\texttt{plus}$。
- 如果 $a - b = c$，请你输出 $\texttt{minus}$。
- 如果以上两条均不满足，请输出 $\texttt{illegal}$。

## 输入格式
输入只有一行三个整数，依次表示 $a,b,c$。

## 输出格式
输出一行一个字符串表示答案。

```input1
1 2 3
```

```output1
plus
```

```input2
3 2 1
```

```output2
minus
```

```input3
1 1 4
```

```output3
illegal
```

## 提示
### 数据规模与约定

对全部的测试点，保证 $-2^{31} \leq a,b,c < 2^{31}$，$b \neq 0$。

