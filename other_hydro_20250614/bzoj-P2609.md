


## 题目描述
**Bytel ** 公司开始生产一种串 **-** 并联电路，每个这样的电路包含很多相连的电子单元以及两个电源，一个串 **-** 并联电路可能有以下组成 **: ** 
**** 
**
这些电路都将组装在一个双面的电路板上。现在的问题就是要确定哪些电路印在正面和哪些印在反面。因为一些技术原因电路应该尽量多的印在反面，但是要求每个单元至少要有一条连接的线路印在正面。求怎样规划使得印在正面的线路最少。
** 
## 输入格式
电路的定义由以下的递归方式进行: 
<ul type="disc">

<li class="MsoNormal" style="margin: 0cm 0cm 0pt; text-align: left; mso-pagination: widow-orphan; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; tab-stops: list 36.0pt; mso-list: l0 level1 lfo1">如果第一行有一个大写字母<tt> **S** </tt> 和一个整数n (2 <= n <= 10000) ，那么这个电路将由n个小的串-并联电路串联在一起构成，这些小网络紧接着在下面的行进行描述, 
<li class="MsoNormal" style="margin: 0cm 0cm 0pt; text-align: left; mso-pagination: widow-orphan; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; tab-stops: list 36.0pt; mso-list: l0 level1 lfo1">如果第一行有一个大写字母<tt> **R** </tt> 和一个整数n (2 <= n <= 10000) ，那么这个电路将由n个小的串-并联电路并联在一起构成，这些小网络紧接着在下面的行进行描述, 
<li class="MsoNormal" style="margin: 0cm 0cm 0pt; text-align: left; mso-pagination: widow-orphan; mso-margin-top-alt: auto; mso-margin-bottom-alt: auto; tab-stops: list 36.0pt; mso-list: l0 level1 lfo1">如果一行只有一个大写字母<tt> **X** </tt> 那么这个电路仅有一个电子单元. 
大写字母<tt> **X** </tt> ** ** 的出现总数不会超过 **10000000, ** 递归的层数最大不超过 **500.** 
## 输出格式
输出仅一个数，表示最少有多少线路印在正面. 

```input1
R 3
S 2
X
R 2
S 2
X
X
S 2
X
X
S 3
X
X
X
R 2
X
X

```
```output1

8
```

## 提示
没有写明提示
## 题目来源
没有写明来源


