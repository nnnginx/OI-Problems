## 题目描述
![](https://cdn.luogu.com.cn/upload/image_hosting/c7b5cigq.png)

Sheila is a student and she drives at ypical student car: it is old, slow, rusty, and falling apart. Recently,the needle on the speedometer fell off. She glued it back on, but she might have placed it at the wrong angle. Thus, when the speedometer reads $s$,her true speed is $s+c$, where $c$ is an unknown constant(possibly negative).

Sheila made a careful record of a recent journey and wants to use this to compute $c$ . The journey consisted of $n$ segments. In the $i^{th}$ segment she traveled a distance of $d_{i}$ and the speedometer read $s_{i}$ for the entire segment. This whole journey took time $t$ . Help Sheila by computing $c$ .

Note that while Sheila's speedometer might have negative readings, her true speed was greater than zero for each segment of the journey.



## 输入格式


The first line of input contains two integers $n (1 \le n \le 1 000)$ , the number of sections in Sheila's journey, and $t (1 \le t \le 10^{6}),$ the total time. This is followed by $n$ lines, each describing one segment of Sheila's journey. The $i^{th}$ of these lines contains two integers $d_{i} (1 \le d_{i} \le 1 000)$ and $s_{i} (|s_{i}| \le 1 000)$ , the distance and speedometer reading for the $i^{th}$ segment of the journey. Time is specified in hours, distance in miles, and speed in miles per hour.



## 输出格式


Display the constant $c$ in miles per hour. Your answer should have an absolute or relative error of less than $10^{−6}.$



## 题目大意
在你面前的是一个坏掉的速度表，当显示速度为 $s$ km/h 时，实际速度为 $s+c$ km/h，$c$ 为固定的常数，为任意实数。你打算计算这个 $c$，于是准备用这个速度表记录速度。现在你要走 $n$ 段路程，第 $i$ 段路程距离为 $d_i$ 米，显示的指数为 $s_i$ km/h，总共路程用了 $t$ 小时。求 $c$ 的值。

你的答案应该与正确答案的差在 $10^{-6}$ 以内。

$1 \le n \le 1000$，$1 \le t \le 10^6$，$1 \le d_i \le 1000$，$|s_i| \le 1000$。

翻译者：一只书虫仔

```input1
3 5
4 -1
4 0
10 3

```

```output1
3.000000000

```

```input2
4 10
5 3
2 2
3 6
3 1

```

```output2
-0.508653377

```

## 提示
Time limit: 1 s, Memory limit: 512 MB. 

spj provider:@[shenyouran](/user/137367).

