## ��Ŀ����
Farmer John's nemesis, Farmer Nhoj, has $N$ cows ($1 \leq N \leq 10^5$), conveniently numbered $1 \dots N$. They have unexpectedly turned up at Farmer John's farm, so the unfailingly polite Farmer John is attempting to give them gifts.

To this end, Farmer John has brought out his infinite supply of gifts, and Nhoj's cows have queued up in front of him, with cow $1$ at the head of the queue and cow $N$ at the tail. Farmer John was expecting that at every timestep, the cow at the head of the queue would take a gift from Farmer John and go to the tail of the queue. However, he has just realized that Nhoj's cows are not that polite! After receiving her gift, each cow may not go to the tail of the queue, but rather may cut some number of cows at the tail, and insert herself in front of them. Specifically, cow $i$ will always cut exactly $c_i$ cows ($0 \leq c_i \leq N-1$).


Farmer John knows that some cows might receive multiple gifts; as he has an infinite supply, this does not worry him. But he is worried that some cows might become unhappy if they do not get any gifts.


Help Farmer John find the number of cows who never receive any gifts, no matter how many gifts are handed out.

## �����ʽ
The first line contains a single integer, $N$.

The second line contains $N$ space-separated integers $c_1, c_2, \dots, c_N$.


## �����ʽ
Please output the number of cows who cannot receive any gifts.


## ��Ŀ����
### ��Ŀ����

Farmer John ������ͷ Farmer Nhoj �� $N$ ͷ��ţ��$1 \leq N \leq 10^5$�������Ϊ $1 \dots N$����������س����� Farmer John ��ũ�������һ����ò�� Farmer John ��ͼ�����������

Ϊ�ˣ�Farmer John �ó��������޵����﹩Ӧ��Nhoj ����ţ������ǰ�ų�һ�ӣ���ţ $1$ �ڶ��ף���ţ $N$ �ڶ�β��Farmer John ԭ����Ϊ����ÿһʱ�̣����׵���ţ��� Farmer John ��������һ�����Ȼ���ߵ���β��Ȼ�������ո���ʶ�� Nhoj ����ţ������ô��ò��ÿͷ��ţ���յ�����󣬿��ܲ����ߵ���β�����ǿ��ܻ��ӵ���β��ĳЩ��ţǰ�档������˵����ţ $i$ ���ǻ��ӵ�ǡ�� $c_i$ ͷ��ţǰ�棨$0 \leq c_i \leq N-1$����

Farmer John ֪����Щ��ţ���ܻ��յ������������������޵����﹩Ӧ���Ⲣ���������ġ��������ĵ��ǣ������Щ��ţû���յ��κ�������ǿ��ܻ��ò����ġ�

����� Farmer John �ҳ������ͳ�����������޷��յ��κ��������ţ������

### �����ʽ

��һ�а���һ������ $N$��

�ڶ��а��� $N$ ���ÿո�ָ������� $c_1, c_2, \dots, c_N$��

### �����ʽ

������޷��յ��κ��������ţ������

```input1
3
1 2 0
```

```output1
1

```

