## ��Ŀ����
Goneril is a very sleep-deprived cow. Her day is partitioned into $n \ (3 \le  n \le  3830)$ equal time periods but she can spend only $b \ (2 \le  b < n)$ not necessarily contiguous periods in bed. Due to her bovine hormone levels, each period has its own utility $u_i \ (0 \le  u_i \le  2\times 10^5)$, which is the amount of rest derived from sleeping during that period. These utility values are fixed and are independent of what Goneril chooses to do, including when she decides to be in bed. With the help of her alarm clock, she can choose exactly which periods to spend in bed and which periods to spend doing more critical items such as writing papers or watching baseball. However, she can only get in or out of bed on the boundaries of a period. She wants to choose her sleeping periods to maximize the sum of the utilities over the periods during which she is in bed. Unfortunately, every time she climbs in bed, she has to spend the first period falling asleep and gets no sleep utility from that period. The periods wrap around in a circle;if Goneril spends both periods $n$ and $1$ in bed, then she does get sleep utility out of period $1$. What is the maximum total sleep utility Goneril can achieve?

������һֻ�ǳ�ȱ������ţ������һ�챻ƽ���ָ�� $n$ �Σ�������Ҫ�����е� $b$ ��ʱ��˯����ÿ��ʱ�䶼��һ��Ч��ֵ $u_i$��ֻ�е���˯����ʱ�򣬲Żᷢ��Ч�á��������ӵİ������������ѡ�������ʱ����˯����Ȼ����ֻ����ʱ�仮�ֵı߽紦��˯��������������ʹ����˯��Ч�õ��ܺ���󡣲��ҵ��ǣ�ÿһ��˯�ߵĵ�һ��ʱ��׶ζ��ǡ���˯���׶Σ�����������Ч��ֵ��ʱ��׶��ǲ���ѭ����Բ��һ��һ����ѭ����������籴����ʱ�� $n$ ��ʱ�� $1$ ˯������ô�����õ�ʱ�� $1$ ��Ч��ֵ��
## �����ʽ
* Line $1$: Two space-separated integers: $n$ and $b$.
* Lines $2\dots n+1$: Line $i+1$ contains a single integer,$u_i$, between $0$ and $2\times 10^5$ inclusive.
* ��һ�У�����������$n$ �� $b$��
* �ڶ��� $n+1$ �У�ÿ�� $1$ �����֣�������ʱ�� $i$ ��Ч��ֵ��
## �����ʽ
* Line $1$: A single integer, the maximum total sleep utility Goneril can achieve.
* ����Ч��ֵ��
```input1
5 3
2
0
3
1
4
```
```output1
6
```
## ����˵��
ѡ��ʱ��� $1$����˯����$4$��$2$��
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$3 \leq n \leq 3830$��$2 \leq b<n$��$0 \leq u_i \leq 2\times 10^5$��
## ��Ŀ��Դ
�����Ҷ� 2005 Twb�� ZgL ��ҵ  
Gold