# AT_abc032_b [ABC032B] 高橋君とパスワード

## 题目描述

高桥君的公司里有一个秘密的金库。由于这个金库需要密码才能进入，而高桥君已经忘记了这个密码。但是幸运的是，他的手边有这个密码的提示，提示是以下这样写的。


- 密码为这张纸上写着的字符串s的长为k的某个子串。

高桥君只需试完所有可能的密码就能打开金库，他因此很高兴~但是，字符串s非常长因此密码的可能情况有很多种。很明显，重复的密码没有必要再试一遍。所有在亲自将所有密码试一遍之前，需要数出有多少种不同的密码。

你的任务就是将给定的字符串s中需要试的相异密码的个数告诉高桥君。

字符串s的“子串”指，字符串s里所含的一段区间的字符取出所得字符串。例如：$abc$的子串有：$a$,$b$,$c$,$ab$,$bc$,$abc$。而请注意，像$ac$或$ba$这样的字符串并非$abc$的子串。

## 输入格式

输入遵从以下形式：

  $ s $  
  $ k $  
  
- 第一行给定的是纸上写有的字符串s，也就是密码的提示。$(1≤length(s)≤300)$s中只含a-z小写英文字母。
- 第二行给定的是密码的长度k$(1≤k≤300)$。k可能比s的长度更大。

## 输出格式

输出按照以下格式。

在第一行输出可能的密码总数。别忘了在最后换行。

# 输入输出样例

## 输入样例#1： 
```
abcabc
2
```
## 输出样例#1： 
```
3
```
## 输入样例#2： 
```
aaaaa
1
```
## 输出样例#2： 
```
1
```
## 输入样例#3： 
```
hello
10
```
## 输出样例#3： 
```
```

翻译提供者：Delva000

## 输入输出样例 #1

### 输入 #1

```
abcabc
2
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
aaaaa
1
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
hello
10
```

### 输出 #3

```
0
```