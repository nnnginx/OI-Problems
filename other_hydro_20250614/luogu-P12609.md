## 题目背景
Score: 15.

## 题目描述
You are spending the day at the CEMC's funfair. One of the rides at the funfair is a roller coaster which has one train with a number of cars. Each car holds the same number of people.

When you arrive at the roller coaster, you see that there is a line. Your job is to determine whether or not you will be on the next train ride, assuming that every car is fully occupied for every ride.

![](https://cdn.luogu.com.cn/upload/image_hosting/21u2ygag.png)

## 输入格式
The first line of input contains a positive integer, $N$, representing your place in line. For example, if $N$ is $5$ then you are the fifth person in line.

The second line contains a positive integer, $C$, representing the number of cars the train has.

The third line contains a positive integer, $P$, representing the number of people a single car
holds.

## 输出格式
Output either `yes` or `no`, indicating whether or not you will be on the next train ride.

```input1
14
3
2
```

```output1
no
```

```input2
12
4
3
```

```output2
yes
```

## 提示
**Explanation of Output for Sample Input 1**

The train has 3 cars and each car holds 2 people. Therefore, 6 people can ride the next train. Since you are the 14th person in line, you will not be on the next train ride.

**Explanation of Output for Sample Input 2**

The train has 4 cars and each car holds 3 people. Therefore, 12 people can ride the next train. Since you are the 12th person in line, you will be on the next train ride.

