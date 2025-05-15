## 题目描述

「恺撒加密」是这样一种加密方式：它将明文中所有字母向后 “位移” $k$ 得到密文

比如若 $k=2$，明文为 `abc`，则密文为 `cde`

若位移超出 Z/z 则回到 A/a，比如若 $k=2$，明文为 `xyz`，则密文为 `zab`

现在给出 $k$ 和一行字符串 $s$，假设 $s$ 是由恺撒加密得到的密文，请**还原其明文**

## 输入格式

输入共两行，第一行包含一个整数 $k$

第二行为一行字符串，只可能包含**大写和小写字母**、**半角逗号句号**、**空格**

## 输出格式

输出一行字符串，表示输入字符串对应的明文

## 样例数据

**样例一**

*input*

```
2
cdeZAB
```

*output*

```
abcXYZ
```

**样例二**

*input*

```
7
Rvuwhrb Fvbtb
```

*output*

```
Konpaku Youmu
```

**样例三**

*input*

```
5
Mnwtfwn Xmttyx F Xywfslj Gnwi, Ynqq Bmjs ...
```

*output*

```
Hiroari Shoots A Strange Bird, Till When ...
```

## 数据范围与约定

对于 $100\%$ 的数据，$0\leq k\leq 25$。输入字符串长度 $\leq 200$