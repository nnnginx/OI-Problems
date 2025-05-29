## 题目背景
保先生是个好司机，总是开车带学生们上山玩。但是去年保先生去年开了最后一趟车后,由于一些奇奇怪怪的原因转行了。半年间，再也没有从这条路上山的人了。

当 VFleaKing 再次来到这座山玩的时候，发现已经没有往日的来来往往的游人了。

算了，过去保先生还在的时候，来山上玩的人，也不全是来欣赏山上的风景的。

![](./2710/file/pica.jpg)

## 题目描述
<u>如果机房马上要关门了，或者你急着要和 MM 约会，请直接跳到第六个自然段。</u>


VFleaKing 注意到了这条上山下山的土路，有些地方能欣赏到美景，有些地方则不能。把上山的道路每 $10cm$ 分为一小段，则对于每一小段，用 $a$ 表示能欣赏到美景，用 $b$ 表示不能欣赏到美景，就能得到一个只含 $a,b$ 的字符串 $s$。当然由于下山和上山是一条路，所以下山的道路的字符串就是将上山的道路的字符串反过来。设上山字符串长度为 $n$，每个字符依次为 $s_1,s_2,\cdots,s_n$。在上山和下山的路上，VFleaKing 会选择某些小段查看旁边的景色，其他时间低头走路。即 VFleaKing 会选择 $k$ 个小段 $x_1,x_2,\cdots,x_k$，且 $k>0,1\le x_1<x_2<\cdots<x_k\le n$，VFleaKing 上山和下山的过程中会在这些地方查看景色。

![](./2710/file/picb.jpg)

VFleaKing 希望，上山下山时看到的美景的情况相同。也就是说，VFleaKing 上山时是否看到了美景的情况是：$s_{x_1},s_{x_2},\cdots,s_{x_k}$，记为字符序列 $T_1$，下山时是否看到了美景的情况是：$s_{x_k},s_{x_{k-1}},\cdots,s_{x_1}$，记为字符序列 $T_2$。VFleaKing 希望 $T_1=T_2$。

VFleaKing 还希望，上山下山时查看景色的间隔相等。也就是说，上山时查看景色的间隔为：$x_2-x_1,x_3-x_2,\cdots,x_k-x_{k-1}$，记为数列 $P_1$。下山时查看景色的间隔为：$x_k-x_{k-1},x_{k-1}-x_{k-2},\cdots,x_2-x_1$，记为数列 $P_2$。VFleaKing 希望 $P_1=P_2$。

VFleaKing 觉得，如果第一次查看景色和最后一次查看景色这段时间里，没有一次低头看路他就会摔倒。也就是说，如果对于所有 $1\le i\le k$ 都有 $x_i=x_1＋i-1$ ，VFleaKing 就会摔倒，VFleaKing不希望发生这样的情况。

<u>就是要在一个只含 $\underline{a,b}$ 的字符串中选取一个子序列，使得：</u>

1. <u>位置和字符都关于某条对称轴对称。</u>

2. <u>不能是连续的一段。</u>


以 $s="abaaaaabbabbabaa"$ 为例。如果我们用符号 $[a_1,a_2,\cdots,a_k]$ 表示一个序列，那么 $[1,4]$ 就是一个合法的序列 $x,[5,8,10,12,15]$ 也是，$[4,5,8,9,10,11,12,15,16]$ 也是。但是 $[1,2]$ 不满足 VFleaKing 第一个希望和第三个希望，所以不是。$[1,2,4]$ 不满足第二个希望，所以不是。$[9,10,11]$ 不满足第三个希望，所以不是。

$Table1:[1,4]$ 是一个合法的序列 $x$ ，关于第 $2$ 列和第 $3$ 列之间的那条夹缝对称
<table>

    <tr>

        <td><font color="red">1</font></td>

		<td><font color="black">2</font></td>

		<td><font color="black">3</font></td>

		<td><font color="red">4</font></td>

		<td><font color="black">5</font></td>

		<td><font color="black">6</font></td>

		<td><font color="black">7</font></td>

		<td><font color="black">8</font></td>

		<td><font color="black">9</font></td>

		<td><font color="black">10</font></td>

		<td><font color="black">11</font></td>

		<td><font color="black">12</font></td>

		<td><font color="black">13</font></td>

		<td><font color="black">14</font></td>

		<td><font color="black">15</font></td>

		<td><font color="black">16</font></td>

    </tr>

    <tr>

        <td><font color="red">a</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black">a</font></td>

		<td><font color="red">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>a</center></font></td>

    </tr>

</table>


$Table2:[5,8,10,12,15]$ 是一个合法的序列 $x$ ，关于第 $10$ 列对称
<table>

    <tr>

        <td><font color="black">1</font></td>

		<td><font color="black">2</font></td>

		<td><font color="black">3</font></td>

		<td><font color="black">4</font></td>

		<td><font color="red">5</font></td>

		<td><font color="black">6</font></td>

		<td><font color="black">7</font></td>

		<td><font color="red">8</font></td>

		<td><font color="black">9</font></td>

		<td><font color="red">10</font></td>

		<td><font color="black">11</font></td>

		<td><font color="red">12</font></td>

		<td><font color="black">13</font></td>

		<td><font color="black">14</font></td>

		<td><font color="red">15</font></td>

		<td><font color="black">16</font></td>

    </tr>

    <tr>

        <td><font color="black">a</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="red">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="red">b</font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="red"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="red"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="red"><center>a</center></font></td>

		<td><font color="black"><center>a</center></font></td>

    </tr>

</table>


$Table3:[4,5,8,9,10,11,12,15,16]$ 是一个合法的序列 $x$ ，关于第 $10$ 列对称
<table>

    <tr>

        <td><font color="black">1</font></td>

		<td><font color="black">2</font></td>

		<td><font color="black">3</font></td>

		<td><font color="red">4</font></td>

		<td><font color="red">5</font></td>

		<td><font color="black">6</font></td>

		<td><font color="black">7</font></td>

		<td><font color="red">8</font></td>

		<td><font color="red">9</font></td>

		<td><font color="red">10</font></td>

		<td><font color="red">11</font></td>

		<td><font color="red">12</font></td>

		<td><font color="black">13</font></td>

		<td><font color="black">14</font></td>

		<td><font color="red">15</font></td>

		<td><font color="red">16</font></td>

    </tr>

    <tr>

        <td><font color="black">a</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black">a</font></td>

		<td><font color="red">a</font></td>

		<td><font color="red">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="red">b</font></td>

		<td><font color="red">b</font></td>

		<td><font color="red"><center>a</center></font></td>

		<td><font color="red"><center>b</center></font></td>

		<td><font color="red"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="red"><center>a</center></font></td>

		<td><font color="red"><center>a</center></font></td>

    </tr>

</table>


$Table4:[1,2]$ 的字符不对称，而且还是连续的，所以不合法
<table>

    <tr>

        <td><font color="red">1</font></td>

		<td><font color="red">2</font></td>

		<td><font color="black">3</font></td>

		<td><font color="black">4</font></td>

		<td><font color="black">5</font></td>

		<td><font color="black">6</font></td>

		<td><font color="black">7</font></td>

		<td><font color="black">8</font></td>

		<td><font color="black">9</font></td>

		<td><font color="black">10</font></td>

		<td><font color="black">11</font></td>

		<td><font color="black">12</font></td>

		<td><font color="black">13</font></td>

		<td><font color="black">14</font></td>

		<td><font color="black">15</font></td>

		<td><font color="black">16</font></td>

    </tr>

    <tr>

        <td><font color="red">a</font></td>

		<td><font color="red">b</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>a</center></font></td>

    </tr>

</table>


$Table5:[1,2,4]$ 位置不对称，所以不合法
<table>

    <tr>

        <td><font color="red">1</font></td>

		<td><font color="red">2</font></td>

		<td><font color="black">3</font></td>

		<td><font color="red">4</font></td>

		<td><font color="black">5</font></td>

		<td><font color="black">6</font></td>

		<td><font color="black">7</font></td>

		<td><font color="black">8</font></td>

		<td><font color="black">9</font></td>

		<td><font color="black">10</font></td>

		<td><font color="black">11</font></td>

		<td><font color="black">12</font></td>

		<td><font color="black">13</font></td>

		<td><font color="black">14</font></td>

		<td><font color="black">15</font></td>

		<td><font color="black">16</font></td>

    </tr>

    <tr>

        <td><font color="red">a</font></td>

		<td><font color="red">b</font></td>

		<td><font color="black">a</font></td>

		<td><font color="red">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>a</center></font></td>

    </tr>

</table>


$Table6[9,10,11]$ 字符和位置都对称，但是是连续的一段，所以不合法
<table>

    <tr>

        <td><font color="black">1</font></td>

		<td><font color="black">2</font></td>

		<td><font color="black">3</font></td>

		<td><font color="black">4</font></td>

		<td><font color="black">5</font></td>

		<td><font color="black">6</font></td>

		<td><font color="black">7</font></td>

		<td><font color="black">8</font></td>

		<td><font color="black">9</font></td>

		<td><font color="black">10</font></td>

		<td><font color="black">11</font></td>

		<td><font color="black">12</font></td>

		<td><font color="black">13</font></td>

		<td><font color="red">14</font></td>

		<td><font color="red">15</font></td>

		<td><font color="red">16</font></td>

    </tr>

    <tr>

        <td><font color="black">a</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">a</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black">b</font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>b</center></font></td>

		<td><font color="black"><center>a</center></font></td>

		<td><font color="red"><center>b</center></font></td>

		<td><font color="red"><center>a</center></font></td>

		<td><font color="red"><center>a</center></font></td>

    </tr>

</table>


给你字符串 $s$，现在 VFleaKing 想知道，有多少个合法的 $x$。答案可能很大，VFleaKing 想知道结果对 $1000000007$ 取模的值。

## 输入格式
一行，一个只包含 $a,b$ 两种字符的字符串。

## 输出格式
一行，一个非负整数表示问题的答案。

## 样例输入#1
```plain
abaabaa
```

## 样例输出#1
```plain
14
```

## 样例输入#2
```plain
aaabbbaaa
```

## 样例输出#2
```plain
44
```

## 样例输入#3
```plain
aaaaaaaa
```

## 样例输出#3
```plain
53
```

## 样例解释#1
$14$ 个方案分别是：
- $[1,3],[1,4],[2,5],[1,6],[3,6],[4,6],[1,7],[3,7],[4,7]$
- $[1,4,7],[3,5,7]$
- $[1,3,4,6],[1,2,5,6],[3,4,6,7]$

## 样例解释#2
我已经想到了一个绝妙的解释，可惜方案太多，写不下了。

## 样例解释#3
我已经想到了一个绝妙的解释，可惜方案太多，写不下了。

## 数据规模与约定
其中 $10\%$ 的数据，字符串仅包含字母 $a$ 或字母 $b$。

另有 $20\%$ 的数据，$n \le 10^3$。

另有 $20\%$ 的数据，要么 $a$ 的个数不超过 $10$，要么 $b$ 的个数不超过 $10$。

另有 $10\%$ 的数据，$n \le 10^4$。

对于 $100\%$ 的数据，$n \le 10^5$。

## 题目来源
2013湖北互测week1