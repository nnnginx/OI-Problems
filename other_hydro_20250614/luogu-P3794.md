## ��Ŀ����
�ⳡ�������������ⱳ�����ܳ�������Ͳ�д�����ˡ� ![](https://cdn.luogu.com.cn/upload/pic/1436.png)


## ��Ŀ����
����һ������Ϊ $n$ ������ $[a_1,a_2\cdots a_n]$������ÿ����������������


����Ҫ�ҳ��ж��ٶ� $(i,j)$��$1 \leq i \leq j \leq n$ ��$\gcd(a_i,a_{i+1}...a_j) \operatorname{xor} (a_i \operatorname{or} a_{i+1} \operatorname{or} \cdots \operatorname{or} a_j)=k$������ $\operatorname{xor}$ ��ʾ���������$\operatorname{or}$ ��ʾ�����ƻ�


## �����ʽ
��һ���������� $n,k$��

�ڶ��� $n$ ������ $a_1,a_2\cdots a_n$��


## �����ʽ
����Ϸ��� $(i,j)$ �Ķ�����


```input1
5 6
2 4 3 4 2
```

```output1
8
```

## ��ʾ
- ���� $30\%$ �����ݣ�$n \leq 500$��
- ���� $60\%$ �����ݣ�$n \leq 100000$��
- ���� $100\%$ �����ݣ�$1 \leq n,a_i \leq 500000$��


