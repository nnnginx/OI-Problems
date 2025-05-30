## 题目描述
小球球是个可爱的孩子，他喜欢玩具，另外小球球有个大大的柜子，里面放满了玩具，由于柜子太高了，每天
小球球都会让妈妈从柜子上拿一些玩具放在地板上让小球球玩。 这天，小球球把所有的 $n$ 辆玩具摆成一排放在
地上，对于每辆玩具 $i$，小球球都会给它涂上一个正整数 $value_{i}$，以表示小球球对该玩具的喜爱程度，$value_{i}$ 越
小则表示他越喜爱。当然对于两辆不同的玩具 $u,v(u\neq v)$，亦有可能 $value_{u}=value_{v}$，也就是说小球球对 $u,v$ 两车的喜爱程度是一样的。小球球很贪玩，他希望能从中间某个位置，连续的取出 $k$ 辆玩具，使得这 $k$ 辆车里喜爱程
度最大的一辆车的喜爱程度正好等于 $k$，且这 $k$ 辆车中没有两辆车的喜爱程度是相同的。小球球希望知道 $k$ 的最大
值为多少。
## 输入格式
第一行一个整数 $n$，表示小球球拥有的玩具数量。    
接下来 $n$ 行，每行一个整数，表示 $value_{i}$。
## 输出格式
一个整数 $k$，即答案。
## 样例输入
```plain
6
2
4
1
3
2
1
```
## 样例输出
```plain
4
```
## 数据规模与约定
$1\leq value_{i}\leq 1\times 10^6$，     
对于 $10\%$ 的测试数据，$n \leq 1 \times 10^5$；        
对于 $100\%$ 的测试数据，$n \leq 1 \times 10^6$。