## ��Ŀ����
The cows have purchased a yogurt factory that makes world-famous Yucky Yogurt. Over the next $n \ (1 \le n \le 10^4)$ weeks, the price of milk and labor will fluctuate weekly such that it will cost the company $c_i \ (1 \le c_i \le 5\times 10^3)$ cents to produce one unit of yogurt in week $i$. Yucky's factory, being well-designed, can produce arbitrarily many units of yogurt each week. Yucky Yogurt owns a warehouse that can store unused yogurt at a constant fee of $s \ (1 \le s \le 100)$ cents per unit of yogurt per week. Fortuitously, yogurt does not spoil. Yucky Yogurt's warehouse is enormous, so it can hold arbitrarily many units of yogurt. Yucky wants to find a way to make weekly deliveries of $y_i \ (0 \le y_i \le 10^4)$ units of yogurt to its clientele ($y_i$ is the delivery quantity in week $i$). Help Yucky minimize its costs over the entire Nweek period. Yogurt produced in week $i$, as well as any yogurt already in storage, can be used to meet Yucky's demand for that week.

ţ���չ���һ�����ҹ������������� $n$ �������ţ�̼۸�������۸񲻶�������� $i$ �ܣ�����һ����λ������Ҫ $c_i$ ��ʿ��������һ����ջ������һ��λ���ң�ÿ����Ҫ $s$ ��ʿ��������ò���仯����ջʮ��ǿ�󣬿��Դ������������ң����ұ�֤���ǲ����ʡ������ӵ��������ڵ� $i$ ����Ҫ���� $y_i$ ��λ�����Ҹ�ί���ˡ��� $i$ �ܸ����������ң��Լ�֮ǰ�Ĵ������������Ϊ��Ʒ���������ţ�Ǽ������ʱ��������������С���ۡ�
## �����ʽ
* Line $1$: Two space-separated integers, $n$ and $s$.
* Lines $2\dots n+1$: Line $i+1$ contains two space-separated integers: $c_i$ and $y_i$.
* ��һ�������������� $n$ �� $s$��
* ������ $n$ ������ $c_i$ �� $y_i$��
## �����ʽ
* Line $1$: Line $1$ contains a single integer: the minimum total cost to satisfy the yogurt schedule. Note that the total might be too large for a 32-bit integer.
* ������ٵĴ��ۡ�ע�⣬���ܳ��� 32 λ�����͡�
```input1
4 5
88 200
89 400
97 300
91 500
```
```output1
126900
```
## ����˵��
�� $1$ ������ $200$ ��λ���Ҳ�ȫ���������� $2$ ������ $700$ ��λ������ $400$ ��λ���� $300$ ��λ���� $3$ �ܽ��� $300$ ��λ������� $4$ ������������ $500$ ��λ��
## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1\le n\le 10^4$��$1 \leq c_i \leq 5\times 10^3$��$1 \leq s \leq 100$��$0 \leq y_i \leq 10^4$��
## ��Ŀ��Դ
Gold