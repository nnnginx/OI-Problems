## ��Ŀ����
Every morning when they are milked, the Farmer John's cows form a rectangular grid that is $R (1 \leq R \leq 10,000)$ rows by $C (1 \leq C \leq 75)$ columns. As we all know, Farmer John is quite the expert on cow behavior, and is currently writing a book about feeding behavior in cows. He notices that if each cow is labeled with an uppercase letter indicating its breed, the two-dimensional pattern formed by his cows during milking sometimes seems to be made from smaller repeating rectangular patterns.

Help FJ find the rectangular unit of smallest area that can be repetitively tiled to make up the entire milking grid. Note that the dimensions of the small rectangular unit do not necessarily need to divide evenly the dimensions of the entire milking grid, as indicated in the sample input below.

## �����ʽ
- Line $1$: Two space-separated integers: $R$ and $C$

- Lines $2\dots R+1$: The grid that the cows form, with an uppercase letter denoting each cow's breed. Each of the $R$ input lines has $C$ characters with no space or other intervening character.

## �����ʽ
- Line 1: The area of the smallest unit from which the grid is formed

## ��Ŀ����
**����Ŀ������**

ÿ�����ϼ���ʱ��ũ��Լ������ţ���ų�һ�� $R (1 \leq R \leq 10,000)$ �г� $C (1 \leq C \leq 75)$ �еľ�������������֪��Լ��ũ����һ���൱�ó�ţ��Ϊ��ר�ң�Ŀǰ����׫дһ��������ţ������Ϊ���顣��ע�⵽�����ÿͷ��ţ������һ����ʾ��Ʒ�ֵĴ�д��ĸ����ô��ţ�ڼ���ʱ�γɵĶ�άͼ����ʱ�ƺ����ɸ�С���ظ�����ͼ����ɵġ�

����Լ��ũ���ҵ������ظ�������������������������С����ľ��ε�Ԫ����ע�⣬С���ε�Ԫ�ĳߴ粻һ����Ҫ��ȫ����������������ĳߴ磬�������ʾ��������ʾ��

**�������ʽ��**

- ��һ�У������ÿո�ָ���������$R$ �� $C$
- �� $2\dots R+1$ �У���ţ�γɵ�����ÿ����ţ��Ʒ���ô�д��ĸ��ʾ��ÿ�� $R$ �������� $C$ ���ַ���û�пո����������ַ���

**�������ʽ��**

��һ�У��γ��������С��λ�����

**����ʾ˵����**

�����������������ͼ�� AB ���ظ�������

���������ڣ�ChatGPT��

```input1
2 5 
ABABA 
ABABA

```

```output1
2
```

## ��ʾ
The entire milking grid can be constructed from repetitions of the pattern `AB`.

