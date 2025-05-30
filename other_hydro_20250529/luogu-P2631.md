## 题目背景
code-11 是一种条形码编码系统，用来将一个字符串编码为条形码。

## 题目描述
在这种编码系统中

可以使用的字符仅有数字0 到9 以及"-"号，以及特殊的start/stop 字符放在条形码的开头

和结尾。对于每个字符，都对应了一个长度为5 的01 串如下所示，对应到条形码中，每个

条形码都是由黑白相隔的条带组成的，且第一个条带为黑色。条带分为宽和窄两种，宽带的宽度为窄带的两倍，0 表示窄的，1 表示宽的条带。

character               Encoding

0                           00001

1                           10001

2                           01001

3                           11000

4                           00101

5                           10100

6                           01100

7                           00011

8                           10010

9                           10000

-                            00100

Start/Stop                00110

而每两个相邻的字符之间一定是一个白色窄带作为分隔。

为了能够检测条形码的正确性，我们加入两个检测数字C 和K，加在条形码的末尾(在

stop 之前)。设需编码的字符串为c1...cn,则C 为：

n
（  ∑     (（n-i）mod 10 +1）\*w(ci)) mod 11

     i=1

K 为：

n+1
（   ∑    (（n-i）mod 10 +1）\*w(ci)) mod 11

      i=1

而cn+1 即为C。其中w(ci)为每个字符的权重。0 到9 即为0 到9。"-"为10。

举个例子，对于字符串123-45，C 和K 分别等于5 和2，则条形码为123-4552，并在前

后加上start 和stop 符号。

在实际应用中，通过探测器探测出每个条带的宽度后，通过解析软件将条形码还原为原本的字符串。

由于条形码方向并未固定，所以软件必须自己判断这个条形码是从左至右的还是从右至左的。 现在，你的任务是扫描并解析一个条形码。你所拥有的信息为每个条带的宽度，但由于设备总是会有误差的，所以，宽带宽度不一定严格的是窄带的宽度的两倍，你的程序需要能够容忍5%的误差。

## 输入格式
由于输出的特殊情况较多，所以采用多组测试数据。 输入第一行包括一个整数T表示测试数据的组数，对于每组数据首先是一个整数n表示该条形码有多少条带。接着n个整数d1..dn以空格隔开表示了每个条带的宽度。再次强调你并不知道这个条形码是从左至右的还是从右至左的，你需要正着和反着都判断一遍。 T <= 20, n <= 150, di<=200。

## 输出格式
对于每组数据输出一行。 输出时分如下几种情况。若该条形码合法，则输出解析所得的原字符串，不包括检测字符C和K。若可以成功解析但是检测字符C错了，则输出"bad C"。若C也是对的，但K是错的，则输出"bad K"。对于剩下所有情况输出bad code。


```input1
3 
59 
10 20 20 10 10 10 20 10 10 20 10 10 10 10 20 10 20 10 10 10 20 10 20 10 20 10 20 10 10 10 10 10 20 10 10 10 10 10 10 20 20 10 20 10 10 20 10 10 20 10 10 10 20 10 10 20 20 10 10 
35 
10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 10 
35 
10 10 20 20 10 10 20 10 10 10 20 10 10 20 10 10 20 10 10 10 20 10 20 10 20 10 10 10 10 10 10 10 20 20 10
```

```output1
123-45 
bad code
bad K
```
## 提示
注意A相对于B误差<=%5是指|A-B|/B<=5%  本题是指宽带相对于窄带。

