# AT_abc149_e [ABC149E] Handshake

## 题目描述

Takahashi  作为特殊嘉宾参加一个晚会 , 晚会上还有 N 个非特殊嘉宾 , 第 i  个特殊嘉宾有 A_i  的欢乐值.晚会目前的欢乐值是 0 .  
 Takahashi  想跟非特殊嘉宾握 M  次手来提高晚会的欢乐值.每一次握手可以被描述为以下的操作:  
1.  Takahashi  选择两个非特殊嘉宾 x  和 y   
2.  Takahashi  用左手和 x  握手 , 用右手和 y  握手 , 晚会的欢乐值增加 A_x + A_y .    

然而 ,  Takahashi  不能以同一种握手方式握两次手.也就是说 ,  Takahashi  的 M  次握手必须满足以下条件:  
- 假设在第 k  次握手中 ,  Takashi  握了非特殊嘉宾 x_k  的左手和 y_k  的右手 , 则没有一组 p  ,  q  (  1 ≤ p < q ≤ M)  可以满足 (  x_p  ,  y_p  ) = (  x_q  ,  y_q  ) .  

请问:在 M  次握手后 , 晚会的欢乐值最大是多少 ?

## 输入格式

第一行: N  ,  M   
第二行: A_1  ,  A_2  , ··· ,  A_N

## 输出格式

一行 , 最大的欢乐值  


---
[翻译者的个人中心](https://www.luogu.com.cn/user/324250)  
[翻译者的博客](https://324250.blog.luogu.org)

## 输入输出样例 #1

### 输入 #1

```
5 3
10 14 19 34 33
```

### 输出 #1

```
202
```

## 输入输出样例 #2

### 输入 #2

```
9 14
1 3 5 110 24 21 34 5 3
```

### 输出 #2

```
1837
```

## 输入输出样例 #3

### 输入 #3

```
9 73
67597 52981 5828 66249 75177 64141 40773 79105 16076
```

### 输出 #3

```
8128170
```