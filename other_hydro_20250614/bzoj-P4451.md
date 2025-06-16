


## 题目描述
给你一个n*n矩阵的第一行和第一列，其余的数通过如下公式推出： 
F[i,j]=a*f[i,j-1]+b*f[i-1,j]+c 
求f[n][n]%(10^6+3) 
## 输入格式
第一行三个数n，a，b，c 
第二行n个数，第i个表示f[i][1] 
第三行n个数，第i个表示f[1][i] 
## 输出格式
仅一个数表示f[n][n]%(10^6+3) 

```input1Sample Input1: 
3 0 0 0 
0 0 2 
0 3 0 
Sample Input2: 
4 3 5 2 
7 1 4 3 
7 4 4 8 

```

```output1Sample Output1: 
0 

Sample Output2: 
41817 
数据范围： 
2<=n<=200000 
其余的数大于等于0小于等于10^6 
```

## 提示
题解:[JudgeOnline/upload/201603/4451.rar](/JudgeOnline/upload/201603/4451.rar)
## 题目来源
没有写明来源


