## ��Ŀ����
��ţ��


## ��Ŀ����
Bessie the cow is competing in a cross-country skiing event at the winter Moolympic games.  She starts out at a speed of 1 meter per second. However, as she becomes more tired over time, she begins to slow down. Each time Bessie slows down, her speed decreases: she moves at 1/2 meter per second after slowing down once, then 1/3 meter per second after slowing down twice, and so on.

You are told when and where Bessie slows down, in terms of a series of events.  An event like this:

T 17
means that Bessie slows down at a specific time -- here, 17 seconds into the race.  An event like this:

D 10
means that Bessie slows down at a specific distance from the start -- in this case, 10 meters.

Given a list of N such events (1 <= N <= 10,000), please compute the amount of time, in seconds, for Bessie to travel an entire kilometer.  Round your answer to the nearest integer second (0.5 rounds up to 1).

�������ڲμ�һ�ѩ������������������ʱ���ٶȺ㶨Ϊÿ�� 1 �ס�Ȼ�������ű������̵����ӣ����᷸�ܶ����ÿ��ʧ�󶼻�ʹ�����ٶ��½���������һ��ʧ����ٶȻ��½���ÿ��1/2 �ף��ڶ���ʧ����ٶȻ��½���ÿ�� 1/3 �ף��� k ��ʧ����ٶȻ��½���ÿ�� 1/(k + 1) �ס�

Լ����¼�˱���������ʧ��һ���� N ����������ʧ��һ�ַ����ڱ�����ʼ���ĳ��ʱ��㣬��һ�ַ�����������ĳ��λ���ϡ���ʱ������������ĳ��ʱ��㵽��ĳ��λ�ã���ǡ�������ʱ����λ���϶���һ��ʧ��ļ�¼����������¼Ҫ������ͬ��ʧ�󣬻�Ա������ٶ��������Ӱ�졣�������յ��������� 1000 �ף����ʱ�����Ҫ����ʱ����ܻ����յ㣿


## �����ʽ
��һ�У��������� N ��1 �� N �� 10000

�ڶ��е��� N + 1 �У�ÿ�п�ͷ�и���д��ĸ����������һ��ʧ�����ͣ�

�C ����� T������������һ������ S����ʾ�ڱ�����ʼ��ĵ� S ������������һ��ʧ��

1 �� S �� 10^7

�C ����� D������������һ������ X����ʾ�ھ������ X �״�������һ��ʧ��1 �� X ��

1000

## �����ʽ
������������ʾ������Ҫ��������ܻ����յ㣬�����ȷ��ʱ�䲻��������������������ķ�

������ӽ�������ȡ��


```input1
2
T 30
D 10
```

```output1
2970
```

## ��ʾ
ǰ 10 �룬�������ٶ���ÿ�� 1 �ף������� 10 �ס�Ȼ���������˵�һ��ʧ���ڽ���

���� 20 ���ڣ����ֻ��� 10 �ס�֮���������˵ڶ���ʧ�󣬻�ʣ�� 980 �ף����������ƻ�ȥ

10 + 20 + 2940 = 2970 �����ɱ���


