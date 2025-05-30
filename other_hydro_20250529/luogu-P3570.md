## 题目描述
Byteburg is a beautiful town by a river.

There are $n$ houses along the river, numbered downstream with successive integers from $1$ to $n$.

Byteburg used to be a nice quiet town in which everyone was happy.

Alas, this changed recently, as two dangerous criminals - Bitie and Bytie set up shop in it.

They did so many robberies already that the citizens are afraid to leave their houses.

Bitie and Bytie do no mere burglaries but rather whole raids: each time they leave their houses and walk towards each other, never turning back.

Bitie walks downstream (towards larger numbers) while Bytie walks upstream (towards smaller numbers).

Along the way, before they meet, each chooses several houses to break into and steal precious items    (and vital data).

After the robberies they meet in a house and divide their loot.

Byteburgers are sick of this already - they would all rather have their tranquility restored.

So they asked the detective Bythony for help.

The detective established that the bandits live in houses of the same color but he does not know which one.

Just a moment ago, an anonymous tip claimed that the robbers are on a raid.

Fearing for their own safety, the source did not say which houses will be broken into.

They did however specify their colors.

As it turns out, the bandits are quite superstitious - each of them will rob a house of each color at most once.

Bythony can wait no longer.

He intends to ambush the criminals at their meeting place.

Aid Bythony in his undertaking by writing a program to find all possible meeting places of the robbers.


## 输入格式
There are two integers in the first line of the standard input, $n$ and $k$ ($3\le n\le 1\ 000\ 000$, $1\le k\le 1\ 000\ 000$, $k\le n$),  separated by a single space, that specify the number of houses and the number of house colors  in Byteburg respectively.

The colors are number with successive integers from $1$ to $k$.

In the second line of input, there is a sequence of $n$ integers, $c_1,c_2,\cdots,c_n$ ($1\le c_i\le k$), separated by single spaces.

These are the colors of successive houses in Byteburg.

In the third line of input, there are two integers $m$ and $l$($1\le m,l\le n$,$m+l\le n-1$), separated by a single space, specifying the numbers of houses (to be) broken into by Bitie and Bytie respectively. In the fourth line of input, there are $m$ pairwise different integers $x_1,x_2,\cdots,x_m$($1\le x_i\le k$), separated by single spaces. These are the colors of houses robbed by Bitie in the order of being broken into (i.e., excluding Bitie's house). In the fifth, which is the last, line of input, there are $l$ pairwise different integers $y_1,y_2,\cdots,y_l$ ($1\le y_i\le k$), separated by single spaces. These are the colors of houses robbed by Bytie in the order of being broken into (again, these do not include Bytie's house). Moreover, $x_m=y_l$ is the color of the house in which the robbers will divide the plunder. (Clearly, they have to break into that one as well!)


## 输出格式
Your program it to print exactly two lines to the standard output.

The first of those should give the number of houses in which the criminals can meet  while respecting aforementioned constraints.

The second line should contain the increasing sequence of the numbers of those houses,  separated by single spaces.

If the robbers cannot meet at all, the first line should contain the number 0 while the second one should be empty.


## 题目大意
## 题目描述

两个罪犯 Bitie 和 Bytie 抢劫 $n$ 个房子，每个房子有一个颜色，Bitie 从低编号到高编号，Bytie 从高编号到低编号，直到相遇为止。已知罪犯开始时所在房子颜色相同（但不知道是什么颜色），并且知道罪犯依次抢劫的所有房子的颜色，且每个罪犯对每种颜色的房子分别最多抢劫一次，求所有可能的相遇点。

## 输入格式

第一行两个整数 $n,k$ ，分别表示房子的个数和不同的颜色数。颜色以从 $1$ 到 $k$ 的整数标号。

接下来一行有 $n$ 个整数 $c_1,c_2,...,c_n (1 \le c_i \le k)$，表示房子的颜色。

第三行有两个整数 $m,l (1 \le m,l \le n,m+l \le n-1)$，分别表示 Bitie 和 Bytie 抢劫房子的个数。

第四行有 $m$ 个两两不同的整数 $x_1, x_2, ..., x_m (1 \le x_i \le k)$，表示 Bitie 抢劫房子的颜色（不包括 Bitie 开始时所在房子的颜色）。

第五行有 $l$ 个两两不同的整数 $y_1, y_2, ..., y_l (1 \le y_i \le k)$，表示 Bytie 抢劫房子的颜色 （不包括 Bytie 开始时所在房子的颜色）。

保证 $x_m = y_l$。

## 输出格式

输出两行，第一行一个整数，表示可能相遇的房子个数，第二行升序输出可能相遇的房子编号。

```input1
15 7
2 5 6 2 4 7 3 3 2 3 7 5 3 6 2
3 2
4 7 3
5 3

```

```output1
3
7 8 10

```

