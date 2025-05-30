## 题目描述
The government of Byteland has decided that it is time to connect their little country to the Internet, so that all citizens can participate in programming competitions and watch videos of cute cats. When it was time to build the network backbone of the country, they assigned the company Internet Optimists Inc. with connecting all the $N$ computers of Byteland. The connections were made as direct links between pairs of computers in such a way that any pair of computers are connected by a sequence of links.

Byteland is not a rich country by any means, so to minimize costs the network topology was built in the form of a tree (i.e. there are exactly $N-1$ direct links between computers). Far too late, it was realised that this solution suffers from a serious drawback. If just a single link is broken, the computers of Byteland will be partitioned so that some computers cannot communicate with each other! To improve the reliability of Byteland's network, it was decided that it should at least tolerate if a single link is broken. Your task is to help Internet Optimists Inc. to improve the network in a cheapest way. Given the network topology of Byteland (i.e. which $N-1$ pairs of computers are connected by direct links), find the minimum number of links that need to be added so that the network will still be connected if any single link is broken.

## 输入格式
The first line of input contains a positive integer $N$ ( $N \geq 3$ ) , the number of computers in Byteland. For simplicity, all computers are numbered from $1$ to $N$. Each of the following $N-1$ lines contains a pair of integers $a$ and $b$ ( $1\leq a,b \leq n,a \ne b$ ) that describes a direct link between computers $a$ and $b$.

## 输出格式
In the first line of output your program should write an integer $k$, the minimal number of links that should be added to the network. In each of the following $k$ lines your program should write a pair of integers $a$ and $b$ ( $1\leq a,b \leq n,a \ne b$ ) that denote the numbers of computers that should be connected by a link. The links can be written in any order. If there is more than one solution, your program should output any one of them.

## 题目大意
### 题目描述### 
拜特朗政府已经决定，现在是时候将他们的小国家与互联网连接起来，以便所有公民都能参加节目比赛，观看可爱猫的视频。当是时候建设这个国家的网络骨干时，他们给互联网乐观主义者公司分配了连接所有N个拜特兰德的电脑。这些连接是作为计算机对之间的直接连接，使任何一对计算机都通过一系列的链接连接起来。

拜特朗是一个发展中国家，因此，为了将成本降到最低，网络拓扑是以树的形式构建的(即有N−1个计算机之间的直接连接)。为时已晚，人们意识到这一解决方案存在严重缺陷。如果只有一个链接断了，那么拜特兰德的计算机就会被分割，这样一些计算机就不能互相通信了！为了提高拜特朗网络的可靠性，人们决定至少要容忍单个链路中断。你的任务是帮助互联网乐观主义者公司以最便宜的方式改进网络。给出了拜特朗的网络拓扑(即N−1个计算机对是通过直接链接连接的)，找到需要添加的最少数量的链接，以便如果任何单个链接中断，网络仍将被连接。

### 输入输出格式
#### 输入格式：
输入的第一行包含一个正整数N(N≥3)，表示拜特兰德的计算机数量。为了简单起见，所有的计算机都是从1到N。以下N−1行包含一对整数。a和b(1≤a, b≤n, a≠b)，它描述计算机之间的直接链接a和b.
#### 输出格式：
在输出的第一行只有一个整数k，表示应该添加到网络中的最少链接数量。在下列每一项中都有对整数。a和b(1≤a ,b≤n ,a≠b)表示应该通过链接连接的计算机数量。链接可以按任何顺序写入。如果有一个以上的解决方案，您的程序应该输出其中的任何一个。

感谢@找寻 提供翻译

```input1
6
1 2
2 3
2 4
5 4
6 4
```

```output1
2
1 5
3 6
```

## 提示
$3 \le N \le 500000$

