# 【题目描述】

芝麻同学国庆想要和父母一起去旅游，他挑选了n个城市，并且查询了相应的航班信息，其中这n个城市通过一些航班来连接。现在芝麻同学的爸爸向芝麻同学提出了一个问题，他想要从出发城市搭乘航班，抵达目的城市的这段旅程花费最少，但是又不想中转太多站，最多经过 k 站中转。你可以帮芝麻同学回答这个问题吗？即找到一条最多经过 k 站中转，并且使得这段旅程的花费最少的路线，并输出该花费；如果不存在这样的路线，则输出 -1。

## 【输入格式】

从文件travel.in中读入数据。

第一行共一个整数 n，表示总共有n个城市。

第二行共一个整数k，表示最多经过k个中转站

第三行共有两个整数src、dst，分别表示芝麻同学的出发城市和要抵达的目的地城市。

第四行共一个整数L，表示L条航班信息

接下来L行，表示航班信息，每一行有三个参数，分别表示起始城市from，终点城市to，起始城市到终点城市的航班价格price。

## 【输出格式】

输出到文件travel.out中。

共一行，输出一个整数，表示出发城市抵达目的地城市的最少花费，若不存在这条航线，输出-1。

# 【样例1输入输出】

```input1
3
1
0 2
3
0 1 100
1 2 100
0 2 500
```

```output1
200
```

# 【样例1解释】

城市航班图如下

![](https://wechatapppro-1252524126.file.myqcloud.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/sspazbln2x3x41.png)

从城市 0 到城市 2 在 1 站中转以内的最便宜价格是 200，如图中红色所示。

# 【样例2输入输出】

```input2
3 
0
0 2
3
0 1 100
1 2 100
0 2 500
```

```output2
500
```

# 【样例2解释】

城市航班图如下

![](https://wechatapppro-1252524126.file.myqcloud.com/appAO5xBfTl4046/image/b_u_60483b946985a_J9JxfeO1/sspazbln2x3x41.png)

从城市 0 到城市 2 在 0 站中转以内的最便宜价格是 500，如图中蓝色所示。

# 【数据范围】

· 1 <= n <= 100

· 0 <= L <= (n * (n - 1) / 2)

· 0 <=from, to < n

· from  != to

· 1 <= price <= 10^4

· 航班没有重复，且不存在自环

· 0 <= src, dst, k < n

· src  != dst

