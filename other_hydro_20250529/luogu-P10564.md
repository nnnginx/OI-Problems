## 题目描述

Bob has many pieces of rubbish. One day, he wants to sort them.
    
    
    
For every piece of rubbish, its type is expressed as a positive integer.
    
    
    
He has $q$ operations. For each operation, it is one of the following two operations.

- `1 s x` He tells you that the piece of rubbish named $s$ has a type of $x$.
- `2 s` He wants to ask you the type of rubbish $s$.


    
But his memories are not always accurate.
    
    
    
For each operation $2$, $s$ may not have appeared in the previous operation $1$s.
    
    
    
We define the similarity of two strings $s_1$ and $s_2$ as $\sum_{i=1}^{\min\{|s_1|,|s_2|\}} [s_{1,i}=s_{2,i}]$.
    
    
    
Here all the strings' indexes start at $1$.
    
    
    
For a string $s$, its type is the type of string which has the maximum similarity to $s$ among all the strings that have appeared in the previous operations $1$s. Note that if there are multiple strings that all have the maximum similarity to $s$, the type of $s$ is the minimum type of these strings' type.
    
    
    
Now, he wants you to solve this problem.
    

## 输入格式

The first line contains an integer $q(1\le q\le 3\times 10^5)$, which is the number of operations.
    
    
    
Next $q$ lines contain operations, one per line. They correspond to the description given in the statement.
    
    
    
It is guaranteed that for every operation $2$ there is at least one operation $1$ before it.
    
    
    
But some pieces of rubbish will have more than one type, you can consider it as the minimum type you have read.
    
    
    
The rubbish's names only consist of lowercase Latin letters.
    
    
    
$1 \le |s| \le 5, 1 \le x \le 10^9$

## 输出格式

    
For every operation $2$, you should print an integer in a single line that is the rubbish $s$'s type.
    

```input1
4
1 aaa 1
2 aa
1 ab 2
2 bb
```

```output1
1
2
```

```input2

```

```output2

```

