## 题目背景
![](https://cdn.luogu.com.cn/upload/image_hosting/tc5is950.png)

## 题目描述
给你两个正整数 $n,m$，你要构造两个正整数 $x,y$（不能有前导 $0$），使得 $x$ 有 $n$ 位，$y$ 有 $m$ 位，且 $x\times y$ 是回文数。

请保证你构造的输出合法，否则后果自负。

## 输入格式
一行两个正整数 $n,m$。

## 输出格式
一行两个整数，表示 $x,y$。

```input1
2 6
```

```output1
83 138017‬

```

```input2
5 5
```

```output2
24513 40723

```

## 提示
对于 $100\%$ 的数据，$n,m \le 10^3$。

**本题采用捆绑测试。**

- Subtask 1(25pts)：$n,m \le 6$。
- Subtask 2(10pts)：$m = 1$。
- Subtask 3(65pts)：无特殊限制。

