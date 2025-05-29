## ��Ŀ����
�������µ������㷨��

```
reverse-sort(sequence a)
    while (a is not in nondecreasing order)
        partition a into the minimum number of slopes
        for every slope with length greater than one
            reverse(slope)
```

���� `slope` Ϊ `a` �ĵݼ��Ӵ���`reverse()` ����תһ�����С�

����һ�� $1$ ~ $N$ �����У���֤�ڵ�һ�λ���ʱÿ�� `slope` �ĳ��ȶ�Ϊż���������ʹ�����������㷨�Ը��������н���������Ҫ���ö��ٴ� `reverse(slope)`��

## �����ʽ
����ĵ�һ�а���һ�������� $N$��

�ڶ��а��� $N$ ��������ͬ�ĵ����������������������С�

## �����ʽ
���һ��һ����������ʾ `reverse(slope)` ��Ҫ�����õĴ�����

```input1
2
2 1
```

```output1
1
```

```input2
4
4 3 2 1
```

```output2
1
```

```input3
4
3 1 4 2
```

```output3
3
```

## ��ʾ
#### �����ݷ�Χ��

���� $100\%$ �����ݣ�$2 \le N \le 10^5$��

#### ��˵����

�����ֵ�� COCI ԭ�����ã����� $140$��

��Ŀ���� **[COCI2011-2012](https://hsin.hr/coci/archive/2011_2012/) [CONTEST #1](https://hsin.hr/coci/archive/2011_2012/contest1_tasks.pdf)** ___T5 SORT___��

