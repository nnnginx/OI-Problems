## ��Ŀ����
Why did the cow cross the road? We may never know the full reason, but it is certain that Farmer John's cows do end up crossing the road quite frequently. In fact, they end up crossing the road so often that they often bump into each-other when their paths cross, a situation Farmer John would like to remedy.

Farmer John raises $N$ breeds of cows ($1 \leq N \leq 100,000$), and each of his fields is dedicated to grazing for one specific breed; for example, a field dedicated to breed 12 can only be used for cows of breed 12 and not of any other breed. A long road runs through his farm. There is a sequence of $N$ fields on one side of the road (one for each breed), and a sequence of $N$ fields on the other side of the road (also one for each breed). When a cow crosses the road, she therefore crosses between the two fields designated for her specific breed.


Had Farmer John planned more carefully, he would have ordered the fields by breed the same way on both sides of the road, so the two fields for each breed would be directly across the road from each-other. This would have allowed cows to cross the road without any cows from different breeds bumping into one-another. Alas, the orderings on both sides of the road might be different, so Farmer John observes that there might be pairs of breeds that cross. A pair of different breeds $(a,b)$ is "crossing" if any path across the road for breed $a$ must intersect any path across the road for breed $b$.


Farmer John would like to minimize the number of crossing pairs of breeds. For logistical reasons, he figures he can move cows around on one side of the road so the fields on that side undergo a "cyclic shift". That is, for some $0 \leq k < N$, every cow re-locates to the field $k$ fields ahead of it, with the cows in the last $k$ fields moving so they now populate the first $k$ fields. For example, if the fields on one side of the road start out ordered by breed as 3, 7, 1, 2, 5, 4, 6 and undergo a cyclic shift by $k=2$, the new order will be 4, 6, 3, 7, 1, 2, 5. Please determine the minimum possible number of crossing pairs of breeds that can exist after an appropriate cyclic shift of the fields on one side of the road.


## �����ʽ
The first line of input contains $N$. The next $N$ lines describe the order, by breed ID, of fields on one side of the road; each breed ID is an integer in the range $1 \ldots N$. The last $N$ lines describe the order, by breed ID, of the fields on the other side of the road.


## �����ʽ
Please output the minimum number of crossing pairs of breeds after a cyclic shift of the fields on one side of the road (either side can be shifted).


## ��Ŀ����
### ��Ŀ����

Ϊʲô��ţҪ����·�����ǿ�����Զ�޷�֪��������ԭ�򣬵����Կ϶����ǣ�Farmer John ����ţȷʵ��������·����ʵ�ϣ����ǹ���·��Ƶ�����֮�ߣ����������ǵ�·������ʱ������ײ���˴ˣ�������� Farmer John ϣ���ܹ����ơ�

Farmer John ������ $N$ ����ţ��$1 \leq N \leq 100,000$��������ÿһ����ض�ר�����ڷ���ĳһ���ض�����ţƷ�֣����磬ר������Ʒ�� 12 �����ֻ������Ʒ�� 12 ����ţ����������������Ʒ�֡�һ����������·�ᴩ����ũ������·��һ����һϵ�� $N$ ����أ�ÿ����ض�Ӧһ��Ʒ�֣�����·����һ��Ҳ��һϵ�� $N$ ����أ�ͬ��ÿ����ض�Ӧһ��Ʒ�֣�����һͷ��ţ����·ʱ��������Ϊ���ض�Ʒ��ָ�����������֮�䴩�С�

��� Farmer John �����ƻ��ø���ϸ�������ܻ�����·���ఴ��ͬ��Ʒ��˳��������أ�����ÿ��Ʒ�ֵ���ؾͻ�ֱ����ԡ��⽫ʹ��ţ����·ʱ����ͬƷ�ֵ���ţ����ײ���˴ˡ�Ȼ������·��������˳����ܲ�ͬ����� Farmer John �۲쵽���ܴ���һЩƷ�ֶԻύ�档һ�Բ�ͬ��Ʒ�� $(a,b)$ �ǡ�����ġ������Ʒ�� $a$ ���κι���··����������Ʒ�� $b$ ���κι���··���ཻ��

Farmer John ϣ����С������Ʒ�ֶԵ���������������ԭ������������ͨ������·һ�����ؽ��С�ѭ����λ�������°�����ţ��λ�á�Ҳ����˵������ĳ�� $0 \leq k < N$��ÿͷ��ţ�����ƶ�����ǰ�� $k$ ����أ���� $k$ ����ص���ţ���ƶ���ǰ $k$ ����ء����磬�����·һ�����������Ʒ��˳��Ϊ 3, 7, 1, 2, 5, 4, 6�������� $k=2$ ��ѭ����λ���µ�˳��Ϊ 4, 6, 3, 7, 1, 2, 5����ȷ���ڶ���·һ�����ؽ����ʵ���ѭ����λ�󣬿��ܴ��ڵĽ���Ʒ�ֶԵ���С������

### �����ʽ

����ĵ�һ�а��� $N$���������� $N$ ����������·һ����ص�Ʒ�� ID ˳��ÿ��Ʒ�� ID �� $1$ �� $N$ ֮������������� $N$ ����������·��һ����ص�Ʒ�� ID ˳��

### �����ʽ

������ڶ���·һ�����ؽ���ѭ����λ�󣨿�����λ����һ�ࣩ������Ʒ�ֶԵ���С������

```input1
5
5
4
1
3
2
1
3
2
5
4
```

```output1
0
```

