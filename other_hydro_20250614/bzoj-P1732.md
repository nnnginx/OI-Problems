## 题目描述
每个城市有 $1000$ 人，要求把给出的 $3\times k$ 个城市分为 $3$ 份，每份 $1000\times k$ 人，每个城市投票人数为 $w_i$，使至少两个城市的票数过半（不包括刚好一半）。
## 输入格式
* Line $1$：一个数 $k$。
* Lines $2\dots 3\times k+1$：每行一个数 $w_i$。
## 输出格式
* Lines $1\dots k$：第一个区域的城市编号。
* Lines $k+1\dots 2k$：第二个区域的城市编号。
* Lines $2k+1\dots 3k$：第三个区域的城市编号。
```input1
2
510
500
500
670
400
310
```
```output1
1
2
3
6
5
4
```
## 样例说明
OUTPUT DETAILS：  
Other solutions might be possible. Note that 「$2\;3$」 would NOT be a district won by the Jerseys， as they would be exactly half of the cows.

## 提示
**本题为 $SJ$**，请暂提交到 http//acm.pku.edu.cn/JudgeOnline/problem?id=2454。
## 题目来源
Gold