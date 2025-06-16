


## 题目描述
<h1 style="margin-top:0cm;margin-right:0cm;margin-bottom:15.0pt;margin-left:
0cm;mso-line-height-alt:13.5pt;background:white">

Everyone knew it would only be a matter of time. So what? Faced for years on, a peril becomes the every-day reality. It loses its meaning...<span lang="EN-US" style="font-size:10.0pt;font-family:Tahoma;
color:#444444">

Today the letter of the Bitotian char Bittard to the Byteotian king Byteasar was released to the public. Bitotia requested annexation of the whole Byteotia on pain of using the Bit Polarizing Magnet (BPM). If used, the BPM would make each and every road in Byteotia unidirectional. The enemy knows only too well that this could be a fatal blow to the minimalist Byteotian infrastructure - there is a unique way between each pair of towns.<span lang="EN-US" style="font-size:10.0pt;font-family:Tahoma;
color:#444444">

How badly can the BPM damage the Byteotian infrastructure? Determine the minimum and the maximum number of such pairs of towns that it will still be possible to travel from one of them to the other while observing the new roads orientation.
给定一棵树，可以对每条边定向成一个有向图，这张有向图的可达点对数为树上有路径从u到达v的点对(u,v)个数。求最小可达点对数和最大可达点对数
<span lang="EN-US" style="font-size:10.0pt;font-family:Tahoma;
color:#444444">

## 
## 输入格式
## The first line of the standard input gives a single integer N （1<=N<=250000）, the number of towns in Byteotia. The N-1 lines that follow describe these roads. Each such line holds two integers, U  and V (1<=U<=V<=N) , which indicate that there is a direct road (still bidirectional at the moment) linking the towns no.  and .
## 

```
## 输出格式


Two integers should be printed to the first and only line of the standard output. The first number should be the minimum and the second - the maximum number of pairs of towns which could remain connected (though in one direction only) after the roads are polarized.
## 
```


```input1
4
1 2
1 3
1 4

```
```output1

3 5
```

## 提示
没有写明提示
## 题目来源
鸣谢HJWJBSR提供译文


