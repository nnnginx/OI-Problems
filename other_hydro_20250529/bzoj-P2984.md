

## 题目描述
给一条长为 $n$ 的纸带，从左到右每个整数的位置标号为 $0,1,2,\cdots,n$，接下来有 $k$ 个操作，每次选取位置 $X$，将整条纸带在 $X$ 处对折。如果 $X$ 是边缘则什么也不做。问最后纸带长度。

## 输入格式

第一行为两个整数代表 $n,k$。

第二行有 $k$ 个整数，表示 $k$ 次对折的位置 $X$。

## 输出格式

一个整数，表示最后纸带的长度。

```input1
9 5 
5 9 2 8 3 

```
```output1
2
```

## 提示
The segment names look as follows:  

Starting situation: $\{0\ 1\ 2\ 3\ 4\ 5\ 6\ 7\ 8\ 9 \}$. 

Consecutively applying the folds:

The segment names look as follows:  

Starting situation: $\{0\ 1\ 2\ 3\ 4\ 5\ 6\ 7\ 8\ 9 \}$. 

Consecutively applying the folds: 
$\to \{0\ (1;9)\ (2;8)\ (3;7\ (4;6)\ 5\} \to \{(1;9)\ (0;2;8)\ (3;7)\ (4;6)\ 5\} \to \{(0;2;8)\ (1;3;7;9)\ (4;6)\ 5\} \to \{(0;2;8)\ (1;3;7;9)\ (4;6)\ 5\} \to \{(1;3;7;9)\ (0;2;4;6;8)\ 5\}$. 
 
 
## 数据规模与约定

对于 $100 \%$ 的数据，$1 \leq k \leq 1\times 10^4$，$1 \leq n \leq 1\times 10^{18}$。

