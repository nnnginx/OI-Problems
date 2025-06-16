## ��Ŀ����
For Bessie the cow��s birthday, Farmer John has given her free reign over one of his best fields to eat grass.

The field is covered in $N$ patches of grass ($1 \le N \le 1000$), conveniently numbered $1\ldots N$, that each have a distinct quality value.  If Bessie eats grass of quality $Q$, she gains $Q$ units of energy.  Each patch is connected to up to 10 neighboring patches via bi-directional paths, and it takes Bessie $E$ units of energy to move between adjacent patches ($1 \le E \le 1,000,000$).

Bessie can choose to start grazing in any patch she wishes, and she wants to stop grazing once she has accumulated a maximum amount of energy.

Unfortunately, Bessie is a picky bovine, and once she eats grass of a certain quality, she��ll never eat grass at or below that quality level again!  She is still happy to walk through patches without eating their grass; in fact, she might find it beneficial to walk through a patch of high-quality grass without eating it, only to return later for a tasty snack.

Please help determine the maximum amount of energy Bessie can accumulate.

## �����ʽ
The first line of input contains $N$ and $E$.  Each of the remaining $N$ lines describe a patch of grass.  They contain two integers $Q$ and $D$ giving the quality of the patch (in the range $1\ldots 1,000,000$) and its number of neighbors.  The remaining $D$ numbers on the line specify the neighbors.

## �����ʽ
Please output the maximum amount of energy Bessie can accumulate.

## ��Ŀ����
### ��Ŀ����

Ϊ����ף��ţ Bessie �����գ�Farmer John ������������õĲݵ������ɳԲݡ�

��Ƭ�ݵر�����Ϊ $N$ ���Ƥ��$1 \le N \le 1000$�������Ϊ $1\ldots N$��ÿ���Ƥ����һ�����ص�����ֵ����� Bessie ��������Ϊ $Q$ �Ĳݣ������� $Q$ ��λ��������ÿ���Ƥͨ��˫��·������� 10 �����ڲ�Ƥ������Bessie �����ڲ�Ƥ֮���ƶ���Ҫ���� $E$ ��λ��������$1 \le E \le 1,000,000$����

Bessie ����ѡ�������һ���Ƥ��ʼ�Բݣ���ϣ���ڻ������������ֹͣ�Բݡ�

���ҵ��ǣ�Bessie ��һͷ���޵�ţ��һ��������ĳ�������Ĳݣ�������Ҳ������������ڻ���ڸ�ˮƽ�Ĳ��ˣ�����Ȼ�����ڲ��Բݵ�����´�����Ƥ����ʵ�ϣ������ܻᷢ�ִ���һ���������Ƥ�����Բ�������ģ�ֻ��Ϊ���Ժ��ٻ���������ζ��С�ԡ�

�����ȷ�� Bessie �ܹ����۵����������

### �����ʽ

����ĵ�һ�а��� $N$ �� $E$���������� $N$ ������ÿ���Ƥ��ÿ�а����������� $Q$ �� $D$���ֱ��ʾ��Ƥ����������ΧΪ $1\ldots 1,000,000$���������ھ�����������ʣ�µ� $D$ ������ָ�����ھӵı�š�

### �����ʽ

����� Bessie �ܹ����۵����������

### ˵��/��ʾ

Bessie �Ӳ�Ƥ 4 ��ʼ����� 5 ��λ��������Ȼ��������·���ƶ�����Ƥ 5�����ƶ������������� 2 ��λ�����������ܾ��Բ�Ƥ 5 �������ϵ͵Ĳݣ��������ƶ�����Ƥ 3���ٴ������� 2 ��λ����������������˲�Ƥ 3 �ϵĲݣ������ 6 ��λ���������ܹ������� 7 ��λ��������

��ע�⣬�����������ύʱ�Ĳ������� 1 ��ͬ��

```input1
5 2
4 1 2
1 3 1 3 4
6 2 2 5
5 2 2 5
2 2 3 4
```

```output1
7
```

## ��ʾ
Bessie starts at patch 4 gaining 5 units of energy from the grass there. She then takes the path to patch 5 losing 2 units of energy during her travel. She refuses to eat the lower quality grass at patch 5 and travels to patch 3 again losing 2 units of energy.  Finally she eats the grass at patch 3 gaining 6 units of energy for a total of 7 energy.

Note that the sample case above is different from test case 1 when you submit.

