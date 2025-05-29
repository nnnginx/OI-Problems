## 题目描述
给定一个 $r\times c$ 的字母矩阵。你需要从这个矩阵的第一行开始，删除尽量多的行， 且保证矩阵任意两列都不相等。输出最多可以删除的行数。

- 两列相等定义为在这两列中同一行的字母都相等。
- 初始的矩阵中任意两列都是不相等的。

## 输入格式
输入第一行两个整数 $r,c$。

接下来的 $r$ 行，每行 $c$ 个字母，描述这个字母矩阵。

保证矩阵中的字母皆为小写字母。

## 输出格式
输出一行一个整数，表示最多可以删除的行数。

```input1
2 6
dobarz
adatak
```

```output1
0
```

```input2
3 4
alfa
beta
zeta
```

```output2
2
```

```input3
4 6
mrvica
mrvica
marica
mateja
```

```output3
1
```

## 提示
#### 数据规模与约定

对于 $100\%$ 的数据，保证 $2\le r,c\le 1000$。

#### 说明

**题目译自 [COCI2010-2011](https://hsin.hr/coci/archive/2010_2011/) [CONTEST #3](https://hsin.hr/coci/archive/2010_2011/contest3_tasks.pdf) *T4 ZNANSTVENIK***。

