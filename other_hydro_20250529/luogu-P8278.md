## ��Ŀ����
$$\begin{aligned}\text{sdjvlajdiofjoiw{\color{1f1e33}n}eglaj}\\\text{pcji{\color{1f1e33}2}gweiruitowoeuri}\\\text{cnvak{\color{1f1e33}5}jflkjweirqoiru}\\\text{rrrwei{\color{1f1e33}f}dlskfjqfafdfaff}\\\text{nmslfjwiejfijlxkjfq{\color{1f1e33}b}el}\\\text{mmm{\color{1f1e33}b}fsfmkdfmksld}\\\text{erjf{\color{1f1e33}n}kerjkwerjkwjeri}\\\text{sdfafafaf{\color{1f1e33}r}fxvzxvzvzx}\end{aligned}$$

## ��Ŀ����
Dream ��һ������Ϊ $n$��$1\le n\le 10^5$�������������� $a_1,a_2,\dots,a_n$�����ж��� $i=1,2,\dots,n$������ $1\le a_i\le 1000$��

��������ǰ׺������ $p_i=a_1+a_2+\dots+a_i$����֤���� **ԭǰ׺������** ������ $1 \le i <n$ ���� $p_i<p_{i+1}$��

���� Tommy ͵������������Լ��� $p$ �����ɸ�Ԫ�����Ϊ $-1$��������ǰ�� $p$ ���飬��ָ�����һ��Ϸ� $a_1,a_2,\dots,a_n$����֤��һ������һ������ $a_i$ ����Ҫ��

## �����ʽ
�����ж������ݣ���һ��һ�������� $t$��Ϊ���������������� $t$ �����ݣ����ж���ÿһ�����ݣ�

��һ��һ������ $n$��

�ڶ��� $n$ ������ $p_i$ ����ǰ׺�����С�

## �����ʽ
����ÿһ�����ݣ�

һ�� $n$ ����������һ������Ҫ��� $a_i$��


```input1
2
5
10 -1 20 -1 30
6
-1 -1 -1 -1 -1 -1
```

```output1
10 5 5 5 5
1 1 4 5 1 4
```

## ��ʾ
#### ���� 1 ����

��������� $a_i$ һ������Ҫ��

- $p_1=10=a_1$��
- $p_3=20=a_1+a_2+a_3$��
- $p_5=30=a_1+a_2+a_3+a_4+a_5$��

#### ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$1\le n,\sum n\le 10^5$������֤��������һ���Ϸ� $a$ ���顣

 - Subtask 1��50 pts�������� $i=1,2,\dots,n$��$p_i\neq -1$��
 - Subtask 2��30 pts������֤������ $i$ ʹ�� $p_i=p_{i+1}=-1$��
 - Subtask 3��20 pts�������������ơ�

