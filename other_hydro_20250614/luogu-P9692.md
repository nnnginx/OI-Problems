## ��Ŀ����
Twenty years ago, the northern section of Beijing Road Pedestrian Street in Guangzhou unearthed eleven layers of pavement from the Tang Dynasty to the Republic of China, and the southern section excavated the foundation of Gongbei Building with five layers from the Song Dynasty to the Ming and Qing Dynasties. This proves that Beijing Road has a long history as a commercial pedestrian street since the Song Dynasty. At the same time, the first Guangdong Province Collegiate Programming Contest was also held at Sun Yat-sen University in Guangzhou. Today, twenty years later, Beijing Road Pedestrian Street has become one of Guangzhou's most famous tourist attractions and shopping destinations, and the Guangdong Province Collegiate Programming Contest is also celebrating its twentieth birthday.

![](https://cdn.luogu.com.cn/upload/image_hosting/qaieoirq.png)

There are $n$ stores in the pedestrian street which buy and sell the same type of product. The buying and selling price of one such product in the $i$-th store are both $a_i$. To avoid over-trading, the pedestrian street has a regulation, that one can only trade $b_i$ times in the $i$-th store (each buy or each sell both count as a trade) and can only trade one product each time.

You're going to earn money by buying and selling the products in the pedestrian street. If you have infinite amount of money at the beginning (that is to say, you can't be short of money when buying a product), what's the maximum total profit you can make? More precisely, \textit{profit} means the total amount of money earned by selling the products, minus the total amount of money spent for buying the products.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 10^5$) indicating the number of stores.

For the following $n$ lines, the $i$-th line contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le 10^6$) indicating the price and the maximum number of trades in the $i$-th store.

It's guaranteed that the sum of $n$ of all test cases will not exceed $10^6$.

## �����ʽ
For each test case output one line containing one integer indicating the maximum total profit.

## ��Ŀ����
**����Ŀ������**

��ʮ��ǰ�����ݵı���·���нֱ��γ��������ƴ�ֱ�����ʱ�ڵ�ʮһ��·�棬�϶��򷢾���δ�������ʱ�ڹ����Ĺ���¥������ַ����֤�˱���·���δ�������Ϊ��ҵ���нֵ��ƾ���ʷ��ͬʱ��һ��㶫ʡ��ѧ��������ƾ���Ҳ��λ�����ݵ���ɽ��ѧ�ٰ졣��ʮ���Ľ��죬����·���н��ѳ�Ϊ�����ʢ���ľ���͹���ʤ��֮һ�����㶫ʡ��ѧ��������ƾ���Ҳӭ�����Լ��Ķ�ʮ�����ա�

�ڲ��н��У��� $n$ ���̵�����ͬһ����Ʒ���� $i$ ���̵�һ����Ʒ���չ��ۺͳ��ۼ۾�Ϊ $a_i$ Ԫ��Ϊ�˷�ֹ���Ƚ��ף����н���һ���涨�����ڵ� $i$ ���̵������� $b_i$ �ν��ף�һ�����һ��������Ϊһ�ν��ף�����ÿ��ֻ�ܽ���һ����Ʒ��

��׼��ͨ���ڲ��н�������������Ʒ��׬Ǯ�������ʼʱ�����޵Ľ�Ǯ��Ҳ����˵��������ΪǮ����������һ����Ʒ������������ڲ��н���׬�����������󣿾�����˵��``����``ָ����������Ʒ��õĽ�Ǯ�ܶ��ȥ������Ʒ���ѵĽ�Ǯ�ܶ

**�������ʽ��**

�ж���������ݡ���һ������һ������ $T$ ��ʾ������������������ÿ��������ݣ�

��һ������һ������ $n$��$1 \le n \le 10^5$������ʾ�̵��������

���ڽ����� $n$ �У��� $i$ �������������� $a_i$ �� $b_i$��$1 \le a_i, b_i \le 10^6$�����ֱ��ʾ�� $i$ ���̵����Ʒ�۸��Լ����̵���Խ��׵���������

��֤�������� $n$ ֮�Ͳ����� $10^6$��

**�������ʽ��**

ÿ���������һ��һ����������ʾ�ڲ��н���׬�������������

**���������͡�**

���ڵ�һ���������ݣ����ŷ������ڵ� $1$ ���̵����� $2$ ����Ʒ���ڵ� $3$ ���̵����� $4$ ����Ʒ���ڵ� $2$ ���̵����� $5$ ����Ʒ���ڵ� $4$ ���̵����� $1$ ����Ʒ��������Ϊ $30 \times 5 + 50 \times 1 - 10 \times 2 - 20 \times 4 = 100$��

���ڵڶ����������ݣ����������̵����Ʒ�۸���ͬ������޷��������

```input1
2
4
10 2
30 7
20 4
50 1
2
1 100
1 1000
```

```output1
100
0
```

## ��ʾ
For the first sample test case, the optimal strategy is to buy $2$ products from the $1$-st store, buy $4$ products from the $3$-rd store, sell $5$ products to the $2$-nd store and sell $1$ product to the $4$-th store. The total profit is $30 \times 5 + 50 \times 1 - 10 \times 2 - 20 \times 4 = 100$.

For the second sample test case, because all stores have the same price, there is no profit.

