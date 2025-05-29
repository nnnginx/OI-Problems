## ��Ŀ����

Farmer John is trying to figure out when his last shipment of feed arrived. Starting with an empty grain bin, he ordered and received $F1$ kilograms of feed. Regrettably, he is not certain exactly when the feed arrived. Of the $F1$ kilograms, $F2$ kilograms of feed remain on day $D$. He must determine the most recent day that his shipment could have arrived. Each of his $C$ cows eats exactly 1 kilogram of feed each day. For various reasons, cows arrive on a certain day and depart on another, so two days might have very different feed consumption.

The input data tells which days each cow was present. Every cow ate feed from Farmer John's bin on the day she arrived and also on the day she left. Given that today is day $D$, determine the minimum number of days that must have passed since his last shipment. The cows have already eaten today, and the shipment arrived before the cows had eaten.

Լ����֪����һ��������ʲôʱ���˵��ģ��������˵�֮ǰ������ţ���ðѲֿ���ԭ��������ȫ�Թ��ˣ����յ������� $F1$ ǧ�����ϣ��ź����ǣ����Ѿ����ǵ�������һ��������ˣ�����$D$��Ϊֹ���ֿ��ﻹʣ�� $F2$ ǧ�����ϣ�

Լ������ $C$ ͷţ��ÿͷţÿ�춼�Ե�ǡ��1ǧ�����ϣ����ڲ�ͬ��ԭ��ţ�Ǵ�ĳһ�쿪ʼ�ڲֿ�����ϣ�����ĳһ���뿪�ֿ⣬���Բ�ͬ��������ܻ��в��ܴ��������������ÿͷţ������������뿪�����춼�ڲֿ�����ϣ� �������������$D$��дһ�������ж��������һ���˵�����ʲôʱ�򣮽���ţ���Ѿ��Թ������ˣ����������˵�������ţ�ǻ�û�гԹ����ϣ�

## �����ʽ

Line $1$ : Four space-separated integers: $C$, $F1$, $F2$, and $D$ .

Lines $2..C+1$ : Line $i+1$ contains two space-separated integers describing the presence of a cow. The first integer tells the first day the cow was on the farm; the second tells the final day of the cow's presence. Each day is in the range $1..2,000$ .

��1�У��ĸ����� $C$��$F1$��$F2$��$D$���ÿո������

��2�� $C+1$ �У�ÿ�����ÿո�������������֣��ֱ��ʾһͷţ���ֿ�����ϵ�ʱ����뿪��ʱ�䣮

## �����ʽ

The last day that the shipment might have arrived, an integer that will always be positive.

һ��������������һ�������˵���ʱ�䣮

```input1
3 14 4 10
1 9
5 8
8 12
```

```output1
6
```

## ���ݹ�ģ��Լ��

�����������ݣ�����

$1<=C<=100$

$1<=F2<=F1<=1,000,000$

$1<=D<=2,000$

## ��ʾ

The shipment was 14 kilograms of feed, and Farmer John has 4 kilograms
left. He had three cows that ate feed for some amount of time in
the last 10 days.

��һ��������14ǧ�����ϣ��������ϻ�ʣ��4ǧ�ˣ����10�����3ͷţ���Թ����ϣ�

Լ���ڵ�6���յ�14ǧ�����ϣ�����Ե�2ǧ�ˣ���7��Ե�2ǧ�ˣ���8��Ե�3ǧ�ˣ���9��Ե�2
ǧ�ˣ���10��Ե�1ǧ�ˣ����û�ʣ4ǧ�ˣ�

## ��Ŀ��Դ
[Silver](http://www.lydsy.com/JudgeOnline/problemset.php?search=Silver)