# Description

小明虽然只有三岁，但是很喜欢数数。有一天，他在一张纸上写了一列两两不同的数。“这些不是一列一般的数，它们是有一定规律的。”小明认真的说。

“经过仔细的观察，你就会发现这些数里隐藏了很多三重逆序数对。所谓三重逆序数对就是指在这列数a1,a2,a3. . .an中，对i<j<k，有ai>aj>ak，那么数对(ai,aj,ak)就称为三重逆序数对。”小明说完后，硬拉着你帮他数一数，他写的数里究竟有多少三重逆序数对。

# Format

## Input

输入文件triple.in的第一行包含一个整数N(1<=N<=100)，即小明写的数的个数。以下N行每行包含一个整数，代表小明所写的一列正整数，不大于30000。

## Output

输出文件triple.out仅包含一个整数M，即小明所写的数中，三重逆序数对的组数。

# Samples

```input1
6
6
1
2 
5
3  
4
```

```output1
2
```


