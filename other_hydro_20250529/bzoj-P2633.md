## ��Ŀ����

�� $n$ ����أ���֪�ҷ���ÿ������ϵ�ʿ���������ҷ�ʿ����Ϊ $0$ ���ʾ��������ҷ�ռ�죬����Ϊ�Է�ռ�졣ĳЩ���֮����ͨ����������Ϊʿ�����Ծ��� $1$ ��λʱ��� $1$ ������ƶ������ڣ���ͨ������������ء�����һ����أ���������ڵ�������з��ҷ���أ����ʾ���ܵ���в����������ҷ�������   
�����󣺶��ҷ�ʿ������һ�� $1$ ����λ���ƶ������������ڱ�֤�ҷ�����ʧ��ص�����£����ҷ�ÿ������ϵ�������Ϊ $0$����ʹ���ҷ������ܵ���в��������������ٵ���ص����������ܶࡣ

## �����ʽ

On the first line a positive integer: the number of test cases, at most 100. After that per test case: 
One line with an integer $n$: the number of regions.   
One line with $n$ integers $a_{i}$: the number of your armies on each region. A number 0 indicates that a region is controlled by your opponents, while a positive number indicates that it is under your control.   
$n$ lines with $n$ characters, where each character is either `Y` or `N`. The $i$-th character of the $j$-th line is `Y` if regions $i$ and $j$ border, and `N` otherwise. This relationship is symmetric and the $i$-th character of the $i$-th line will always be `N`. 
In every test case, you control at least one region, and your opponents control at least one region. Furthermore, at least one of your regions borders at least one of your opponents' regions. 

## �����ʽ

Per test case: 
One line with an integer: the maximum number of armies on your weakest border region after one turn of moving.

```input1
2 
3 
1 1 0 
NYN 
YNY 
NYN 
7 
7 3 3 2 0 0 5 
NYNNNNN 
YNYYNNN 
NYNYYNN 
NYYNYNN 
NNYYNNN 
NNNNNNY 
NNNNNYN

```

```output1
1
4
```

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ����� $1 \leq n \leq  100$��$0 \leq a_{i} \leq 100$��$1 \leq \text{��������} \leq 100$��

## ��Ŀ��Դ

Nwerc2010


