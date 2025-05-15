[Altair](https://music.163.com/song?id=1383924010)

## 题目描述

云浅有一个 $n$ 个点的**无向完全图**，每条边有边权，一开始每条边的边权都是 $0$。

现在你需要进行若干次操作，每次可以选一个三元环 $(x,y,z)$，其中 $x,y,z$ 互不相同，然后把 $(x,y),(y,z),(z,x)$ 三条边的边权都 $+1$。试构造一种操作数在 $[1,10^6]$ 之间的方案，使得操作后图中每条边的边权都相等。如果无解，输出 `-1`。

## 输入格式

**本题有多组数据。**

第一行一个正整数 $T$ 表示数据组数，每组数据会输入一行一个正整数 $n$ 表示图的点数。

## 输出格式

对于每组数据：

- 若无解，输出 $-1$。
- 若有解，你需要先在第一行输出一行一个正整数 $k$ 表示你进行的操作次数，接下来输出 $k$ 行，每行三个正整数 $x,y,z$ 表示这次操作你选择的三元环。

## 样例 $1$ 输入

```
2
3
4
```

## 样例 $1$ 输出

```
1
1 2 3
4
1 2 3
1 2 4
1 3 4
2 3 4
```

## 样例 $1$ 解释

对于第一组数据，可以发现对 $(1,2,3)$ 这个三元环操作一次后，每条边的边权都是 $1$，符合题意。

对于第二组数据，操作四次后每条边的边权都是 $3$，符合题意。

## 校验器

为方便选手调试，我们提供了自定义校验器 `checker.cpp`，该校验器**只会检查你输出的方案是否合法，而不会检验是否无解**。也就是说，只要你对每组数据都输出 `-1`，就可以通过该校验器的检验。**不保证该校验器和实际测试使用的校验器完全相同**。

以下为其源代码，选手可以在 `testlib.h` 的同一目录下自行编译并运行。运行方式为：`checker <input-file> <output-file> <answer-file>`，其中 `<input-file>` 表示输入文件，`<output-file>` 代表你的输出文件，`<answer-file>` 可以是任意文件。

```cpp
#include<bits/stdc++.h>
#include"testlib.h"

using namespace std;

const int LIM=1e6;

int main(int argc,char **argv){
	
	registerTestlibCmd(argc,argv);
	
	int T=inf.readInt();
	while(T--){
		int n=inf.readInt();
		vector<vector<int> >G(n+1,vector<int>(n+1,0));
		int k=ouf.readInt(-1,LIM);
		if(k==-1)continue;
		else if(k==0)quitf(_wa,"Number of operations should be in [1,1000000].\n");
		else{
			for(int i=1;i<=k;i++){
				int x=ouf.readInt(1,n),y=ouf.readInt(1,n),z=ouf.readInt(1,n);
				if(x==y||y==z||z==x)quitf(_wa,"Invalid operation.\n");
				if(x>y)swap(x,y);
				if(x>z)swap(x,z);
				if(y>z)swap(y,z);
				G[x][y]++,G[y][z]++,G[x][z]++;
			}
			for(int i=1;i<=n;i++)for(int j=i+1;j<=n;j++)if(G[i][j]!=G[1][2])quitf(_wa,"Wrong answer.\n");
		}
	}
	quitf(_ok,"Right Output!");

	return 0;
}
```

## 测试点约束

对于所有数据，$3\le n\le 1000,1\le T\le 1000,3\le \sum n\le 2000$。

其中 $\sum n$ 表示所有 $T$ 组数据中的 $n$ 之和。

| 子任务编号 | $n\le$ |  特殊性质  | 依赖子任务  | 分值 |
| :--------: | :----: | :--------: | :---------: | :--: |
| Subtask #1 |  $6$   |     无     |     无      | $5$  |
| Subtask #2 | $100$  |     无     |     $1$     | $15$ |
| Subtask #3 | $350$  |     无     |    $1,2$    | $21$ |
| Subtask #4 | $650$  |     无     |   $1,2,3$   | $13$ |
| Subtask #5 | $1000$ | $n$ 为奇数 |     无      | $10$ |
| Subtask #6 | $1000$ |     无     | $1,2,3,4,5$ | $36$ |


