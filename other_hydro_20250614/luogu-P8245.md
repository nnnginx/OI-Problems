## ��Ŀ����
������������ $A,B$ ֮���**����**Ϊ�������������ж�Ӧλ�ϵ����Ĳ�ľ���ֵ֮�ͣ���Ϊ $\operatorname{dist}(A,B)$���ر�أ���� $A,B$ ������λ������ͬ������λ����С����ǰ����ǰ�� $0$�����磺

- $\operatorname{dist}(4561,3278)=\left|4-3\right|+\left|5-2\right|+\left|6-7\right|+\left|1-8\right|=12$��
- $\operatorname{dist}(32,5678)=\left|0-5\right|+\left|0-6\right|+\left|3-7\right|+\left|2-8\right|=21$��

���ڣ������������� $L,R$������������������� $[L,R]$ �ڵ������Եľ���͡����ڴ𰸿��ܴܺ����**��� $\bf 10^9+7$ ȡģ**��

## �����ʽ
�����һ�У������������� $L,R$��

## �����ʽ
���һ��һ����������ʾ���������� $[L,R]$ �ڵ������Եľ���Ͷ� $\bf 10^9+7$ ȡģ֮���ֵ��

```input1
1 5
```

```output1
40
```

```input2
288 291
```

```output2
76
```

```input3
1000000 10000000
```

```output3
581093400
```

## ��ʾ
**������ 2 ���͡�**

���������� $[288,291]$ �ڵ������Եľ������£�

- $\operatorname{dist}(288,289)=\operatorname{dist}(289,288)=1$��
- $\operatorname{dist}(288,290)=\operatorname{dist}(290,288)=9$��
- $\operatorname{dist}(288,291)=\operatorname{dist}(291,288)=8$��
- $\operatorname{dist}(289,290)=\operatorname{dist}(290,289)=10$��
- $\operatorname{dist}(289,291)=\operatorname{dist}(291,289)=9$��
- $\operatorname{dist}(290,291)=\operatorname{dist}(291,290)=1$��

��˾����Ϊ $2\times (1+9+8+10+9+1)=76$��

**�����ݷ�Χ�����ơ�**

���� $20\%$ �����ݣ����� $A,B\leqslant 10^4$��  
���� $40\%$ �����ݣ����� $A,B\leqslant 10^{100}$��  
�����������ݣ�$1\leqslant A\leqslant B\leqslant 10^{50000}$��

**����Ŀ��Դ��**

������Դ�� **_[COCI 2013-2014](https://hsin.hr/coci/archive/2013_2014/) [CONTEST 3](https://hsin.hr/coci/archive/2013_2014/contest3_tasks.pdf) T5 PAROVI_**������ԭ���������ã����� $140$ �֡�

�� [Eason_AC](https://www.luogu.com.cn/user/112917) ���������ṩ��

