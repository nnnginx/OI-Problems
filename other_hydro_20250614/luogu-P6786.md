## ��Ŀ����
С A ��һ������Ϊ $n$ ������ $a_1,a_2,\cdots,a_n$��

�������Щ����ѡ��һЩ�� $b_1,b_2,\cdots,b_k$ ���㣺�������� $i\ (1\leq i\leq k)$��$b_i$ Ҫô������ $b$ �е����ֵ��Ҫô����һ��λ�� $j$ ʹ�� $b_j>b_i$ �� $b_i+b_j+\gcd(b_i,b_j)=\mathrm{lcm}(b_i,b_j)$��

- ����㲻֪�� $\gcd$ �� $\mathrm{lcm}$ ��ʲô�����Ե����ײ��ġ�����/��ʾ�����ֵ����ӡ�

С A ����ѡ������֮�;����������������ֵ��

## �����ʽ
��һ��һ������ $n$����ʾ���еĳ��ȡ�

�ڶ��� $n$ ������ $a_1,a_2,\cdots,a_n$��

## �����ʽ
���һ��һ��������ʾ�𰸡�

```input1
4
4 3 2 1
```

```output1
5
```

```input2
10
6 7 18 4 17 10 9 1 3 8
```

```output2
19
```

```input3
3
123456789 234567890 123456789
```

```output3
246913578
```

## ��ʾ
**������ 1 ˵����**

����ѡ�� $b=\{2,3\}$����Ϊ $2+3+\gcd(2,3)=\mathrm{lcm}(2,3)$��

**�����ݷ�Χ��Լ����**

**�������������ԡ�**

- Subtask 1��5 points����$n\leq2$��
- Subtask 2��20 points����$n\leq 17$��
- Subtask 3��15 points����$a_i\leq 2\times 10^3$��
- Subtask 4��15 points����$n\leq 2\times 10^3$��
- Subtask 5��10 points����$n\leq 5\times 10^4$��
- Subtask 6��10 points����$a_i\leq 10^7$��
- Subtask 7��25 points�������������ơ�

���� $100\%$ �����ݣ�$1\leq n\leq 3\times 10^5$��$1\leq a_i\leq 10^9$��

**������/��ʾ��**

$\gcd$ ��ʾ[���Լ��](https://baike.baidu.com/item/%E6%9C%80%E5%A4%A7%E5%85%AC%E7%BA%A6%E6%95%B0/869308?fr=aladdin)��$\mathrm{lcm}$ ��ʾ[��С������](https://baike.baidu.com/item/%E6%9C%80%E5%B0%8F%E5%85%AC%E5%80%8D%E6%95%B0/6192375?fr=aladdin)��

**����Դ��**

[��LGR-075����� 8 ������ II Div.2 & SWTR-06 & EZEC Round 3](https://www.luogu.com.cn/contest/33190)��

idea & solution & data by [Alex_Wei](https://www.luogu.com.cn/user/123294)��

