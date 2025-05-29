## ��Ŀ����
Due to recent rains, water has pooled in various places in Farmer John's field, which is represented by a rectangle of N x M (1 <= N <= 100; 1 <= M <= 100) squares. Each square contains either water ('W') or dry land ('.'). Farmer John would like to figure out how many ponds have formed in his field. A pond is a connected set of squares with water in them, where a square is considered adjacent to all eight of its neighbors. Given a diagram of Farmer John's field, determine how many ponds he has.






## �����ʽ
Line 1: Two space-separated integers: N and M \* Lines 2..N+1: M characters per line representing one row of Farmer John's field. Each character is either 'W' or '.'. The characters do not have spaces between them.




## �����ʽ
Line 1: The number of ponds in Farmer John's field.



## ��Ŀ����
���ڽ��ڵĽ��꣬��ˮ�㼯��ũ��Լ������ز�ͬ�ĵط���������һ�� $N\times M(1\leq N\leq 100, 1\leq M\leq 100)$ ������ͼ��ʾ��ÿ����������ˮ��`W`�� ���Ǻ��أ�`.`����һ������������Χ�İ˸�������������һ��������������Ϊһ��ˮ�ӡ�Լ����Ū�����������Ѿ��γ��˶���ˮ�ӡ�����Լ����ص�ʾ��ͼ��ȷ�������ж���ˮ�ӡ�

����� $1$ �У������ո������������$N$ �� $M$��

�� $2$ �е��� $N+1$ �У�ÿ�� $M$ ���ַ���ÿ���ַ��� `W` �� `.`�����Ǳ�ʾ����ͼ�е�һ�š��ַ�֮��û�пո�

���һ�У���ʾˮ�ӵ�������

```input1
10 12
W........WW.
.WWW.....WWW
....WW...WW.
.........WW.
.........W..
..W......W..
.W.W.....WW.
W.W.W.....W.
.W.W......W.
..W.......W.

```

```output1
3

```

## ��ʾ
OUTPUT DETAILS: There are three ponds: one in the upper left, one in the lower left, and one along the right side.


