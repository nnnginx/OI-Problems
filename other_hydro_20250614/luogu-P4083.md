## ��Ŀ����
Bessie and Elsie have each baked $N$ pies ($1 \leq N \leq 10^5$). Each of the $2N$ pies has a tastiness value according to Bessie and a (possibly different) tastiness value according to Elsie.

Bessie is thinking about giving one of her pies to Elsie. If Elsie receives a pie from Bessie, she will feel obligated to give one of her pies to Bessie. So as to not appear stingy nor flamboyant, Elsie will try to pick a pie that is at least as tasty (in Elsie's eyes) as the pie she received, but no more than $D$ units tastier ($0 \leq D \leq 10^9$). Such a pie may not exist, in which case Elsie will adopt a pseudonym and exile herself to Japan.


But if Elsie does give Bessie a pie in return, Bessie will similarly try to give Elsie a pie which is at least as tasty but no more than $D$ units tastier (in Bessie's eyes) as the pie Elsie just gave her. Should this be impossible, Bessie too will exile herself. Otherwise she will give her chosen pie to Elsie. This cycle will continue until one of the cows is exiled, an unhappy outcome, or one of the cows receives a pie which she accords a tastiness value of $0$, in which case the gift exchange will end and both cows will be happy.


Note that a pie may not be gifted twice, nor can either cow return a pie gifted to her.


For each of the $N$ pies Bessie could select as her initial gift to Elsie, determine the minimum number of pies that could possibly be gifted in the resulting exchange before the cows are happy.


## �����ʽ
The first line contains the two integers $N$ and $D$.

The next $2N$ lines contain two space-separated integers each, respectively denoting the value of a particular pie according to Bessie, and the value of that pie according to Elsie.


The first $N$ lines refer to Bessie's pies, and the remaining $N$ lines refer to Elsie's pies.


It is guaranteed that all tastiness values are in the range $[0,10^9]$.


## �����ʽ
There should be $N$ lines in the output. Line $i$ should contain a single integer: the minimum number of pies that could be gifted in a happy gift exchange started with Bessie's pie $i$. If no gift exchange starting with pie $i$ is happy, then line $i$ should contain the single integer $-1$ instead.


## ��Ŀ����
### ��Ŀ����

Bessie �� Elsie ���Կ��� $N$ ���ɣ�$1 \leq N \leq 10^5$������ $2N$ �����е�ÿһ������һ���� Bessie ��������ζֵ��һ�������ܲ�ͬ�ģ��� Elsie ��������ζֵ��

Bessie ���ڿ��ǽ�����һֻ���͸� Elsie����� Elsie �յ��� Bessie ���ɣ����������������� Bessie һֻ�ɡ�Ϊ�˼Ȳ��Ե�����Ҳ���Ե���ҫ��Elsie �᳢��ѡ��һֻ���������������յ�����һ����ζ���������� $D$ ��λ����ζ���ɣ�$0 \leq D \leq 10^9$��������������ɲ����ڣ�Elsie ������һ���������������ŵ��ձ���

����� Elsie ȷʵ������ Bessie һֻ�ɣ�Bessie Ҳ�����Ƶس����͸� Elsie һֻ�������������� Elsie ���͸�������һ����ζ���������� $D$ ��λ����ζ���ɡ�����ⲻ���ܣ�Bessie Ҳ���������š��������Ὣ��ѡ������͸� Elsie�����ѭ����������ֱ������һͷ��ţ�����ţ�һ�������Ľ��������������һͷ��ţ�յ�һֻ��������ζֵΪ $0$ ���ɣ�����������£����ｻ������������ͷ��ţ����е����ˡ�

��ע�⣬һֻ�ɲ��ܱ��������Σ��κ�һͷ��ţҲ���ܻ������յ����ɡ�

���� Bessie ����ѡ����Ϊ��ʼ�����͸� Elsie ��ÿһֻ�ɣ�ȷ������ţ�Ǹе�����֮ǰ�����ܱ����͵��ɵ���С������

### �����ʽ

��һ�а����������� $N$ �� $D$��

�������� $2N$ ��ÿ�а��������ÿո�ָ����������ֱ��ʾĳֻ���� Bessie ��������ζֵ���� Elsie ��������ζֵ��

ǰ $N$ ������ Bessie ���ɣ�ʣ�µ� $N$ ������ Elsie ���ɡ�

��֤������ζֵ���� $[0,10^9]$ ��Χ�ڡ�

### �����ʽ

���Ӧ���� $N$ �С��� $i$ ��Ӧ����һ������������� Bessie �ĵ� $i$ ֻ�ɿ�ʼ�����ｻ���Ǹ��˵ģ���������ܱ����͵��ɵ���С������������� $-1$��

```input1
2 1
1 1
5 0
4 2
1 4
```

```output1
3
1

```

