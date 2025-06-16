## 题目背景
JosephZheng 在写数学作业的预习。他往往使用 Casio 来帮忙解一元二次方程。但是 Casio 有一个问题，就是当 $\Delta=b^2-4ac$ 为一个大素数或大合数时，其开平方的结果会以小数显示，而不是老师要求的二次根式形式。JosephZheng 很是苦恼，一遇到这种情况就要手动解方程。一天他再也忍不住了，于是打开了电脑，编了一个 prime 程序……于是悲剧的 OIer 们就要跟着疯狂的 JosephZheng 一起编这个程序，呵呵……


## 题目描述
废话少说，给你一个大数 $N$（不一定在 int64 范围内），让你进行素性判断，然后分解质因数。当然，初中数学题不可能有大于 int64 的数让你判断素性，因此超过范围的数可以忽略不计。为了让程序更加贴心，JosephZheng 多了一些要求，会在输入输出中给出具体情况。


## 输入格式
一个大数 $N$（$N$ 为非负整数），其中这个数的各个数位之间可以插入各种符号，例如 $1234$ 可以为 `1 - 2alsdkjf3！@￥%！@@@##￥……！￥#-4` 等。你需要在这一长串乱码中找出这个要判断的数。输入数据可能有多组，如果读到一行没有数字的字串即结束。字符串长度可能大于 $255$。


## 输出格式
在读入数据之前先输出 `Enter the number=`，需要换行。

然后输出 `Prime?`，问号后有一个空格，但不要换行。

如果是质数则输出 `Yes!` 否则输出 `No!`。此时换行。

若果是质数就 halt，若是小于 $2$ 的数则在输出 `No!` 后也 halt。若是合数则分解质因数。如果该数大于四千万则输出 `The number is too large!`，然后 halt。否则分解质因数。输出结果的方式在输出样例中会详细给出。每组数据之间空一行。


```input1
4
eed

```

```output1
Enter the number=
Prime? No!
4=2^2

Enter the number=

```

```input2
2
end

```

```output2
Enter the number=
Prime? Yes!

Enter the number=

```

```input3
-1
adfs

```

```output3
Enter the number=
Prime? No!

Enter the number=

```

```input4
1234###24#@13#@￥！1
hehe

```

```output4
Enter the number=
Prime? No!
The number is too large!

Enter the number=

```

```input5
1.5
1
1234324123512343123
@~@~@~@

```

```output5
Enter the number=
Prime? No!
15=3^1*5^1

Enter the number=
Prime? No!

Enter the number=
Prime? No!
The number is too large!

Enter the number=

```

```input6
12
halt@@

```

```output6
Enter the number=
Prime? No!
12=2^2*3^1

Enter the number=

```

## 提示
编这道题的 JosephZheng 有些无聊，但是很考验基本功哦！仔细审题！

水题一道。。。


