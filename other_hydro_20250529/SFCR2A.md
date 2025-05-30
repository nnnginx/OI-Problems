### 题目背景
初三时，小 L 因为道德与法治考试痛苦不堪，于是他开始思考如何让订正和复习的时间之和最小。
### 题目描述
在某次考试中，共有 $n$ 道非选择题，其中第 $i$ 道题**涉及且仅涉及**第 $p_i$ 个知识点。一共有 $m$ 个知识点，编号为 $1 \sim m$。

由于爆零了，小 L 被要求订正这张卷子。对于某个知识点 $x$，你要么选择在卷子上**每道**与它有关的题旁边抄上其对应的知识点，要么选择将其对应的知识点标注在书上**恰好一次**并且在**每道**对应题目旁记录下该知识点在书上的位置。若要将其抄在卷子上，需要花费时间 $a_x$；若要将其在书上标注，需要花费时间 $b_x$；若要将其在书上的位置记录在对应题目旁，需要花费时间 $c_x$。

他假定他在接下来的日子里要复习这张卷子 $k$ 轮。当他在某一轮中复习某道题时，假定其对应知识点为 $x$，若他将知识点 $x$ 抄在了卷子上，他需要用 $d_x$ 的时间背诵这个知识点；否则，他需要用 $e_x$ 的时间在书上找到并背诵这个知识点（**但如果他在这一轮复习中已经背诵过这个知识点了，他不会再背一次**）。

现在他不想订正了，于是他给你 $q$ 个询问，每个询问包含一个整数 $k$，表示求出订正一次和复习 $k$ 次的时间之和的最小值。
### 输入格式
第一行，三个整数 $n, m, q$；

第二行，$n$ 个整数 $p_1, p_2, \cdots, p_n$；

第三行，$m$ 个整数 $a_1, a_2, \cdots, a_m$；

第四行，$m$ 个整数 $b_1, b_2, \cdots, b_m$；

第五行，$m$ 个整数 $c_1, c_2, \cdots, c_m$；

第六行，$m$ 个整数 $d_1, d_2, \cdots, d_m$；

第七行，$m$ 个整数 $e_1, e_2, \cdots, e_m$；

接下来 $q$ 行，每行一个整数 $k$。
### 输出格式
$q$ 行，每行一个整数，表示所求的值。
### 样例 #1
#### 样例输入 #1
```
6 6 3
1 1 4 5 1 4
3 4 5 6 7 8
2 3 4 5 6 7
1 2 3 4 5 6
6 5 4 3 2 1
7 6 5 4 3 2
1
3
5
```
#### 样例输出 #1
```
36
60
83
```
### 数据范围
对于 $10\%$ 的数据，$1 \leq m \leq 10$，$1 \leq q \leq 5 \times 10^3$；

对于 $30\%$ 的数据，$1 \leq m, q \leq 5 \times 10^3$；

对于 $50\%$ 的数据，$1 \leq m, q \leq 10^5$；

对于另 $20\%$ 的数据，$1 \leq k \leq q = 500$；

对于 $100\%$ 的数据，$1 \leq n, m, q \leq 3 \times 10^5$，$1 \leq p_i \leq m$，$1 \leq c_i < b_i < a_i \leq 10^9$，$1 \leq d_i < e_i \leq 5 \times 10^5$，$1 \leq k \leq 10^8$。