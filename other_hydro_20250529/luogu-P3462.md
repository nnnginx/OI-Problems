## 题目描述
While moving to a new compound the Byteotian Institute of Experimental Physics has encountered a logisticalproblem - the transfer of its vast collection of precision weights turned out to be non-trivial.

The Institute has a certain number of containers of limited strength at its disposal. As many weightsas possible are to be put into the containers, the remaining ones will be discarded. There is no limit onthe number of weights to be put in a container apart from the requirement of not exceeding its strength. Acontainer may also be empty.

Any two weights in the Institute have a peculiar property: the mass of one of them is an integer multipleof the mass of the other. Particularly, they may have the same mass.

TaskWrite a programme which:

reads the durabilities of the containers and masses of the weights from the standard input,        determines the maximal number of weights that can be put in the containers,        writes the outcome to the standard output.


## 输入格式
The first line of the standard input contains two integers $n$ and $m$($1\le n,m\le 100\ 000$), separated by a singlespace, denoting respectively: the number of containers and the number of weights. The second line of thestandard input consists of $n$ integers $w_i$ ($1\le w_i\le 1\ 000\ 000\ 000$ for $1\le i\le n$), separated by single spaces,denoting the strengths of containers in milligrammes. In the third line there are $m$ integers $m_j$($1\le m_j\le 1\ 000\ 000\ 000$) for $1\le j\le m$), separated by single spaces, denoting masses of the weights in milligrammes.


## 输出格式
The first and only line of the standard output should contain a single integer -the maximal number ofweights that can be placed in the containers without exceeding their durability.


## 题目大意
在 byteotian 公司搬家的时候，他们发现他们的 $m$ 个大量的精密砝码的搬运是一件恼人的工作。公司有 $n$ 个固定容量的容器可以装这些砝码。他们想装尽量多的砝码以便搬运，并且丢弃剩下的砝码。

每个容器可以装的砝码数量没有限制，但是他们能够装的总重量不能超过每个容器的限制。第 $i$ 个容器允许装下的砝码总重为 $w_i$。一个容器也可以不装任何东西。

此外，这些砝码有一个特征。对于任意两个砝码 $i,j$，它们的重量成倍数关系，即 $m_i\mid m_j$ 或者 $m_j\mid m_i$ 或者两者都成立（即重量相等）。

```input1
2 4
13 9
4 12 2 4
```

```output1
3
```

