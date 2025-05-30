## 题目描述
When Prof. Pang was young, he wrote the following code for quick sort. Please calculate how many swaps are performed when calling $\textbf{quicksort}$$(A, 1, n)$. $A$ is a given permutation with length $n$.

![](https://cdn.luogu.com.cn/upload/image_hosting/8ig9i3bq.png)

## 输入格式
The first line contains one integer $T~(1\le T \le 10^5)$, the number of test cases.

For each test case, the first line contains one positive integer $n~(1\le n \le 5\times 10^5)$. The next line contains $n$ integers $a_1,\ldots, a_n~(1 \le a_i\le n)$ denoting the permutation $A$. It is guaranteed that $a_1,\ldots, a_n$ form a permutation, i.e.~$a_i\neq a_j$ for $i \neq j$. 

It is guaranteed that the sum of $n$ over all test cases is no more than $5\times 10^5$.

## 输出格式
For each test case, output one line containing the number of swaps performed when calling $\texttt{quicksort}(A, 1, n)$.

## 题目大意
### 题目描述

给定一个长度为 $n$ 的排列 $A$。现使用如下伪代码对 $A$ 进行排序：

```
procedure QUICKSORT(A,lo,hi)
    if lo>=0 and hi>=0 and lo<hi then
    	p=PARTITION(A,lo,hi)
        QUICKSORT(A,lo,p)
        QUICKSORT(A,p+1,hi)
    end if
end procedure
procedure PARTITION(A,lo,hi)
    pivot=A[floor((hi+lo)/2)]
    i=lo-1
    j=hi+1
    while True do
        repeat
            i=i+1
        until A[i]>=pivot
        repeat
            j=j-1
        until A[j]<=pivot
        if i>=j then
            return j
        end if
        Swap A[i] with A[j]
    end while
end procedure
```

试计算：调用 `QUICKSORT(A,1,n)` 函数过程中，`Swap` 操作执行了多少次。

### 输入格式

第一行包含一个整数 $T$ $(1\leqslant T\leqslant 10^5)$，表示测试数据组数。

对于每组测试数据：

第一行包含一个正整数 $n$ $(1\leqslant n\leqslant 5\times 10^5)$。

第二行包含 $n$ 个整数 $a_1,\dots,a_n$ $(1\leqslant a_i\leqslant n)$，表示排列 $A$。保证 $a_1,\dots,a_n$ 构成一个排列，即：$\forall i\not= j,a_i\not=a_j$。

保证所有测试数据中 $n$ 的和不超过 $5\times 10^5$。

### 输出格式

对于每组测试数据，输出一行一个整数，表示调用 `QUICKSORT(A,1,n)` 函数过程中，`Swap` 操作执行的次数。

```input1
3
3
3 2 1
5
2 4 5 3 1
10
7 2 4 6 1 9 10 8 5 3
```

```output1
1
4
7
```

