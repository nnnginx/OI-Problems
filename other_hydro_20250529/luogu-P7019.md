## 题目描述


Anna has just finished her course project. She has a lot of seven-segment LED displays as leftovers and a small power source. Each display consumes power proportionally to the number of lit segments, e.g . $‘9'$ consumes twice more power than $‘7'.$

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15131/1.png)

Anna wonders what is the maximum possible sum of digits she is able to achieve, if her power source is able to light $n$ segments, and she wants to light exactly $n$ segments.



## 输入格式


The single line of the input contains one integer $n$ -- the number of segments that should be lit $(2 \le n \le 10^{6}).$



## 输出格式


Output a single integer -- the maximum possible sum of digits that can be displayed simultaneously.



## 题目大意
用 LED 显示器来表示数字，表示方法如下：

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15131/1.png)

你必须正好点亮 $n$ 段 LED 灯，使得这些灯能够组成一些数字。现在请你求出这些一位数和的最大值。

注：“一段”LED 灯指的是一条黑色的纵向短线或一条黑色的横向线段。如，`9` 由 $6$ 断组成。

$2\le n\le2\times 10^6$。

Translated by [cmll02](https://www.luogu.com.cn/user/171487)。

```input1
4

```

```output1
4

```

```input2
7

```

```output2
11

```

```input3
6

```

```output3
14

```

## 提示
Time limit: 3 s, Memory limit: 512 MB. 



