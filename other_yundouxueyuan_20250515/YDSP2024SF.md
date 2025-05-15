## 题目描述
给一张 $n$ 个点的随机无向完全图 $G$，$G$ 的每条边被染上了黑色或者白色。

给定两个 $1$ 到 $n$ 的排列 $a,b$，保证不存在 $1\le i,j<n$ 使得 $a_i=b_j$ 且 $a_{i+1}=b_{j+1}$ 或 $a_i=b_{j+1}$ 且 $a_{i+1}=b_j$（此处且的优先级比或高）。如下构造无向图 $H$：
1. 初始 $H=G$。
2. 对于每个 $i\in[1,n)$，将 $H$ 上的边 $(a_i,a_{i+1})$ 染黑。
3. 对于每个 $i\in[1,n)$，将 $H$ 上的边 $(b_i,b_{i+1})$ 染白。

现在，对于 $[1,n)$ 中的每个正整数 $k$，求一条 $H$ 上的哈密顿路使得其上恰有 $k$ 条黑边。保证有解。
### 输入格式
第一行一个正整数 $n$。

第二行 $n$ 个正整数描述排列 $a$。

第三行 $n$ 个正整数描述排列 $b$。

无向图 $G$ 由如下 C++ 代码生成：
```cpp
// col[u][v] 表示无向边 (u, v) 的颜色：0 表示白色，1 表示黑色
auto popcount = [&](unsigned x)
{
	int ans = 0;
	while (x){++ans; x &= x-1;}
	return ans;
};
auto X = [&](unsigned x)
{
	x ^= x << 13;
	x ^= x >> 7;
	x ^= x << 17;
	return x;
};
for (int i=1; i<=n; i++)
	for (int j=1; j<=n; j++) col[i][j] = popcount(X(i) ^ X(j)) & 1;
```
## 输出格式
$n-1$ 行，每行 $n$ 个正整数，第 $i$ 行按顺序描述你对于 $k=i$ 构造的路径上的点。如果有多种可能解答，输出任意一个即可。
## 样例组
### 输入样例
```plain
5
1 2 3 4 5
1 3 5 2 4
```
### 输出样例
```plain
1 3 4 2 5
4 5 2 3 1
5 3 2 1 4
4 3 2 1 5
```
## 数据范围
共 20 个测试点，对于第 $i$ 个测试点，$n=\lceil 1.4^{i+5}\rceil$，所有测试点均为 5 分。保证不存在 $1\le i,j<n$ 使得 $a_i=b_j$ 且 $a_{i+1}=b_{j+1}$ 或 $a_i=b_{j+1}$ 且 $a_{i+1}=b_j$。

对于某个测试点，如果你答对了 $p\%$ 的 $k$ 对应的路径，你就可以获得 $p\%$ 的分数。注意，如果你不知道某个 $k$ 所对应的路径，你也至少应该在那一行输出 $n$ 个 $1$ 到 $n$ 之间的整数。

选手可以在下发文件获取一份 SPJ 来在本地测试输出正确性（[checker](./5397/file/checker.cpp)、[testlib](./5397/file/testlib.h)）。使用方法：
- 首先将 `testlib.h` 和 `checker.cpp` 置于同一目录下，然后编译 `checker.cpp` 得到可执行文件 `checker.exe`（Windows）或 `checker`（Linux）。
- 如果输入文件是 `<input-file>`、你的输出文件是 `<output-file>`、答案文件是 `<answer-file>`（在本题中只需要在这个位置放一个空文件），在命令行运行：
    ```sh
    checker.exe <input-file> <output-file> <answer-file>   (Windows)
    ./checker <input-file> <output-file> <answer-file>     (Linux)
    ```
    观察输出结果即可获得 `<output-file>` 输出文件的得分。

具体也可以参考 [OI Wiki 上的对应页面](https://oi-wiki.org/tools/testlib/checker/)。