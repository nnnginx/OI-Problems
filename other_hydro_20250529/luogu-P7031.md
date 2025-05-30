## 题目描述


Two students, Adam and Anton, are celebrating two-year anniversary of not passing their Math $Logic exa_m.$ After very careful search in a local supermarket, they bought a rectangular cake with $integer dimensions$ and two candles.

Later in the campus Adam put the candles into different integer points of the cake and gave a knife $to Anto_n$ to cut the cake. The cut should start and end at integer points at the edges of the cake, and $it should$ not touch the candles. Also each piece should have exactly one candle at it. Please, help $Anto_n to$ find the starting and ending points of the cut.

![](https://onlinejudgeimages.s3.amazonaws.com/problem/13473/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202016-11-01%20%EC%98%A4%ED%9B%84%202.30.49.png)

A $7 \times 3$ cake and two candles at $(2 , 2)$ and $(3 , 2)$ .

Anton can cut this cake through $(0 , 0)$ and $(4 , 3)$ .



## 输入格式


The single line of the input contains six integers: $w , h$ -- cake dimensions; $a_{x}, a_{y}$ -- $x$ and $y coordinates$ of the first candle; $b_{x}, b_{y}$ -- the coordinates of the second candle $(3 \le w , h \le 10^{9}; 0 < a_{x}, b_{x} < w$ ; $0 < a_{y}, b_{y} < h$ ; $a_{x} ≠ b_{x}$ or $a_{y }≠ b_{y}).$



## 输出格式


Output four integers $s_{x}, s_{y}, e_{x},$ and $e_{y}$ -- the starting and ending coordinates of the cut. Both $starting and$ ending point of the cut should belong to the sides of the cake.

If there are several solutions, output any of them.



## 题目大意
有一个长方形蛋糕和两个蜡烛，蛋糕的尺寸是整数。

把两个蜡烛放在蛋糕的不同整数点上，并用一把刀来切蛋糕。切割应该在蛋糕边缘的整数点开始和结束，并且不应该接触蜡烛。此外，每件作品都应该有一支蜡烛。请找到切入的起点和终点。

```input1
7 3 2 2 3 2 

```

```output1
0 0 4 3

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 

spj provider:@[shenyouran](/user/137367)

