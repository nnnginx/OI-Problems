## 题目描述


Ian works for a rating agency that publishes ratings of the best universities. Irene is a journalist who plans to write a scandalous article about the upcoming rating.

Using various social engineering techniques (let's not get into more details), Irene received some insider's information from Ian.

Specifically, Irene received several triples $(a_{i}, b_{i}, c_{i}),$ meaning that in the upcoming rating, university $b_{i}$ stands between universities $a_{i}$ and $c_{i}.$ That is, either $a_{i}$ comes before $b_{i}$ which comes before $c_{i},$ or the opposite. All triples told by Ian are consistent -- let's say that actual rating satisfies them all.

To start working on the first draft of the future article, Irene needs to see at least some approximation to the actual rating. She asked you to find a proposal of a rating in which at least half of the triples known by Irene are satisfied.



## 输入格式


The first line contains integers $n$ and $m$ , the number of rated universities, and the number of triples given to Irene by Ian $(3 \le n \le 100 000$ ; $1 \le m \le 100 000)$ .

Each of the next $m$ lines contains three distinct integers $a_{i}, b_{i}, c_{i}$ -- the universities making a triple $(1 \le a_{i}, b_{i}, c_{i} \le n)$ .



## 输出格式


Output the proposal of a rating from the first university to the last one. The proposal rating should satisfy at least $m/2$ triples. If there are many such proposals, output any one of them.



## 题目大意
## 题意

对于 $[1, n]$ 的排列，给 $m$ 个限制，第 $i$ 个限制描述 $b_i$ 出现在 $a_i$，$c_i$ 之间。保证存在一个排列满足所有限制。

构造一个 $n$ 的排列至少满足 $\lceil \frac m2 \rceil$ 个限制。

```input1
4 3
1 2 3
1 2 3
1 4 3

```

```output1
4 3 2 1

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 



