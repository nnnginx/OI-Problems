## ��Ŀ����

Farmer John is constructing a new milking machine and wishes to keep it secret as long as possible. He has hidden in it deep within his farm and needs to be able to get to the machine without being detected. He must make a total of $t \ (1 \le  t \le  200)$ trips to the machine during its construction. He has a secret tunnel that he uses only for the return trips. The farm comprises $n \ (2 \le  n \le  200)$ landmarks (numbered $1\dots n$) connected by $p \ (1 \le  p \le  4\times 10^4)$ bidirectional trails (numbered $1\dots p$) and with a positive length that does not exceed $10^6$. Multiple trails might join a pair of landmarks. To minimize his chances of detection, FJ knows he cannot use any trail on the farm more than once and that he should try to use the shortest trails. Help FJ get from the barn (landmark $1$) to the secret milking machine (landmark $n$) a total of $t$ times. Find the minimum possible length of the longest single trail that he will have to use, subject to the constraint that he use no trail more than once.(Note well��The goal is to minimize the length of the longest trail, not the sum of the trail lengths.) It is guaranteed that FJ can make all $t$ trips without reusing a trail.

Լ����������һ̨���͵ļ��̻���������ϣ������֪������ϣ�������ܾõ�����������ܡ����Ѽ��̻���������ũ���ʹ���������֡��ڼ��̻�����Ĺ����У�����Ҫȥ���̻����ڵĵط� $t$ �Ρ�����ũ���������ܵĵص�����Լ��ֻ�ڷ��ص�ʱ��������ũ�������ֳ� $n$ �������� $1$ �� $200$ ��š���Щ���� $p$ ����·���ӣ�ÿ��·��һ��С�� $10^6$ �ĳ��� $l$����������֮������ж�����·���ӡ�Ϊ�˼��ٱ����ֵĿ��ܣ�Լ���������ξ���ũ���ϵ��κ�һ����·����Ȼ�ˣ���ϣ������̵�·�������Լ��Ѱ���� $t$ �δӲֿ��ߵ����̻����ڵص�·�ߡ��ֿ������� $1$�����̻����ڵ������� $n$����������Ҫ�����Լ����������Щ��·�����·�ĳ�����С�Ƕ��٣���Ȼ�������ظ���ĳһ��·����ע�⣬����Ҫ��Ĳ�����̵���·�̳��ȣ�������������ֱ��������������ĵ�·����ĵ�·����С���ȡ����ݱ�֤Լ�������ҵ� $t$ ��û���ظ��ĴӲֿ⵽���̻����������·��

## �����ʽ

* Line $1$: Three space-separated integers: $n,p$, and $t$.
* Lines $2\dots p+1$: Line $i+1$ contains three space-separated integers,$a_i,b_i$, and $l_i$, indicating that a trail connects landmark $a_i$ to landmark $b_i$ with length $l_i$.
* �� $1$ ���� 3 ������ $n$��$p$ �� $t$���ÿո������
* �� $2$ �� $p+1$ �У�ÿ�а��� 3 ��������$a_i$��$b_i$��$l_i$����ʾ���� $a_i$��$b_i$ ֮����һ������Ϊ $l_i$ �ĵ�·��

## �����ʽ

* Line $1$: A single integer that is the minimum possible length of the longest segment of Farmer John's route.
* ���ֻ��һ�У�����һ����������Լ����������Щ��·�����·����С���ȡ�

```input1
7 9 2
1 2 2
2 3 5
3 7 5
1 4 1
4 3 1
4 5 7
5 7 1
1 6 3
6 7 3
```

```output1
5
```

## ����˵��

Լ��ѡ�� $1\to 2\to 3\to 7$ �� $1\to 6\to 7$ ����·�ߡ���Щ·�����·����С������ $5$��

## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq t \leq 200$��$2 \leq n \leq 200$��$1 \leq p \leq 4\times 10^4$��$0\le l\le 10^6$��
## ��Ŀ��Դ

Gold