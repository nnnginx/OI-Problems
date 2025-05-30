## 题目描述
The participants of the World Programming Competition submitted $N$ solution files $f_1 ,...,f_N$ to the grading system. Before accepting the results as final, the jury would like to rule out any possibility of plagiarism. They have a program that takes two files and compares them to decide if they are too similar to each other.

However, the number of files is rather big and it would take too much time to compare all pairs. On the other hand, many pairs could be quickly eliminated based on the fact that the file sizes are too different.

More precisely, the jury decided to fully skip comparing every pair where the size of the smaller file is less than 90% of the size of the larger one. So, the comparison program has to examine only those distinct pairs of files $(f_i, f_j)$ where $i≠j, size(f_i) \le size(f_j)$ and $size(f_i) \ge 0.9 \times size(f_j)$.

Write a program that computes the number of pairs of files that will have to be examined.

## 输入格式
The first line of input contains the integer $N$, the number of solution files submitted. The second line contains $N$ integers $size(f_1),\cdots,size(f_N)$, each showing the size of one file.

## 输出格式
The first and only line of output must contain one integer, the number of pairs of files that will have to be examined.

## 题目大意
Description

世界编程大赛的选手们提交N份程序文件f1, …, fN给评测系统。在将评测结果正式公布之前，评委会想要排除一切可能的剽窃现象。他们已有一个对比程序，用来比较两份程序文件，并判断它们是否太过相似了。 然而程序文件的数目相当大，把每两份（一对，pair）文件都进行比较的话将花太多的时间。另一方面，许多对(pair)可以直接被排除，如果文件的大小相差太大的话。 更准确地说，评委会决定，如果每两份文件（一对，pair）中，较小文件的体积小于较大文件的体积的90%，那将直接不比较这样的一对(pair)。所以，对比程序只比较这样的一对(fi, fj)： i≠j, size(fi )≤ size(fj )且size(fi )≥0.9∙size(fj )。 编写程序计算有多少对(pair)文件需要被比较。

Input:

第1行包含一个整数N，即提交的程序文件总数。 第2行包含N个整数size(f1), …, size(fN)，每个整数代表文件的体积大小。

Output:

第1行，也是唯一的一行，给出一个整数，即需要被比较的文件的对(pair)的数目。

感谢@谦谦君子 提供翻译

```input1
2
2 1
```

```output1
0
```

```input2
5
1 1 1 1 1
```

```output2
10
```

## 提示
对于 $50\%$ 的数据，$1 \le N \le 2000$。

对于所有数据，$1 \le N \le 10^5,1 \le f_i \le 10^8$。

