


## 题目描述
小C最近在学习线性函数，线性函数可以表示为：f(x) = kx + b。现在小C面前有n个线性函数fi(x)=kix+bi ，他对这n个线性函数执行m次操作，每次可以：
1.M i K B 代表把第i个线性函数改为：f_{i}(x)=kx+b 。
2.Q l r x 返回f_{r}(f_{r-1}(...f_{l}(x)))  mod  10^9+7 。
## 输入格式
第一行两个整数n, m (1 <= n, m <= 200,000)。
接下来n行，每行两个整数ki, bi。
接下来m行，每行的格式为M i K B或者Q l r x。
## 输出格式
对于每个Q操作，输出一行答案。

```input1
5 5
4 2
3 6
5 7
2 6
7 5
Q 1 5 1
Q 3 3 2
M 3 10 6
Q 1 4 3
Q 3 4 4

```

```output1
1825
17
978
98
```

## 提示
<span lang="EN-US" style="font-size:10.5pt;mso-bidi-font-size:
11.0pt;font-family:"Calibri","sans-serif";mso-fareast-font-family:宋体;
mso-bidi-font-family:"Times New Roman";mso-font-kerning:1.0pt;mso-ansi-language:
EN-US;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">1 <= n, m <= 200,000<span style="font-size:10.5pt;mso-bidi-font-size:11.0pt;
font-family:宋体;mso-ascii-font-family:Calibri;mso-hansi-font-family:Calibri;
mso-bidi-font-family:"Times New Roman";mso-font-kerning:1.0pt;mso-ansi-language:
EN-US;mso-fareast-language:ZH-CN;mso-bidi-language:AR-SA">，<span lang="EN-US" style="font-size:10.5pt;mso-bidi-font-size:11.0pt;font-family:"Calibri","sans-serif";
mso-fareast-font-family:宋体;mso-bidi-font-family:"Times New Roman";mso-font-kerning:
1.0pt;mso-ansi-language:EN-US;mso-fareast-language:ZH-CN;mso-bidi-language:
AR-SA">0 <= k, b, x < 1000,000,007
## 题目来源
没有写明来源


