# AT_cf_2015_relay_b 全完

## 题目描述

团队竞赛中合作很重要。现在你要参加一个团队答题接力赛，目标当然是全完(全部问题完美回答)。
这个接力赛是10人一组前往，给出从问题1开始到问题10的10个问题。必须一人回答一问，同一个人不能解多个问题。给出每个成员可以解出的问题列表，判定团队能否解出全部问题。**但是**某个成员解不出的问题，经过可以解出该问题的另一名成员的讲解，就可以解出了。现实中的接力赛还有时限，对于这个问题就无视吧。

## 输入格式

每个成员可以解出的问题列表，以以下标准形式给出：
 ```
 $ p1,1  p1,2...   p1,10 $  
 $ p2,1  p2,2...   p2,10 $  
             :
 $ p10,1  p10,2...   p10,10 $  
```
其中，pi,j只能是"o"或"x"，"o"代表第i名成员可以解出第j个问题。"x"则代表不能解出。

## 输出格式

如果团队可以解出全部问题，则输出"Yes"，否则输出"No"(均不含引号，末尾要输出回车)

## 输入输出样例 #1

### 输入 #1

```
oxxxxxxxxx
xoxxxxxxxx
xxoxxxxxxx
xxxoxxxxxx
xxxxoxxxxx
xxxxxoxxxx
xxxxxxoxxx
xxxxxxxoxx
xxxxxxxxox
xxxxxxxxxo
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
xxxxxxxxxx
oooooooooo
```

### 输出 #2

```
Yes
```

## 输入输出样例 #3

### 输入 #3

```
oxxxxxxxxx
ooxxxxxxxx
ooxoxxxxxx
oooxoxxxxx
oxxxxooxxx
ooxoxxoxxx
oooooxxxxx
ooooxxoxxx
ooooxoxxox
oooooooxxo
```

### 输出 #3

```
No
```

## 说明/提示

样例1: 
可以，每个人解出他们会的一问即可。

样例2: 
可以，第十个人教其他成员所有问题的解法即可。

样例3: 
不可以，第八问无人能解。

感谢@玉签初报明 提供的翻译