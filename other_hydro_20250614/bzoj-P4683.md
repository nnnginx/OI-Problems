


## ��Ŀ����
����
AwD��ү�Ǹ����
��Ŀ
AwD��ү�ֵ���������������
�X�mHFLSyzx���Ա߹�ز���
AwD��ү����������ʵ����̫û����ս���ˣ����Ǳ㿪ʼyy�����Ƶļ�ǿ�桪������ͼ
��������ͼΪÿ���������������򵥻��ϵ�ͼ
���ڳ�ʼ����ͼ�ǿյģ�����Ҫ֧����������
link a b w
���һ������a,b�ıߣ�ȨֵΪw
���������֮��������ͼ�����ok
�������failed�����������β���
cut a b w
ɾ��һ������a,bȨֵΪw�ı�
����ж��ɾ��һ��
��������������ı����failed�������Ա��β���
�������ok
distance? a b
ѯ��a,b֮������·
���a,b����ͨ���-1
AwD��ү�������һ�����ˣ���������һ��
�X�mHFLSyzx������ֱ�����ι�ȥ
Ϊ�˲���AwD��ү��ǰ�������X�mHFLSyzx����A�������
��������ȫ������
����������������
## �����ʽ
��һ��n��m��ʾ��n���ڵ㣬m������
������m�У�ÿ��һ������
��֤�ض�Ϊlink cut����distance?
m <= 300000,���й��ڱ߳��ļ�����int��Χ��
n <= 100000
�п������رߣ��п���Ȩֵһ�����رߣ�
�п���link�Ի�����ʱ���failed
�п���ѯ��������ͬ�ĵ�����·����ʱ���0
## �����ʽ
��ÿ���������һ�У�����ò����Ľ��/��

```input1
��������1
5 12
link 1 2 3
link 2 3 3
distance? 1 3
cut 2 3 3
distance? 1 3
cut 2 3 2
link 2 3 2
cut 2 3 3
link 3 4 3
link 4 1 5
link 1 3 8
link 2 4 7
��������2
6 25
link 1 2 3
link 1 2 2
link 1 2 5
cut 1 2 2
cut 1 2 5
link 1 2 3
link 1 2 3
cut 1 2 3
cut 1 2 3
cut 1 2 3
cut 1 2 3
link 1 2 4
link 1 3 5
distance? 2 3
link 2 4 1
link 3 4 2
link 2 3 3
link 1 4 7
link 1 4 7
cut 1 4 7
link 5 6 8
distance? 3 6
distance? 2 6
cut 2 4 1
distance? 1 5

```
```output1
�������1
ok
ok
6
ok
-1
failed
ok
failed
ok
ok
ok
failed



�������2
ok
ok
ok
ok
ok
ok
ok
ok
ok
ok
failed
ok
ok
9
ok
ok
ok
failed
failed
failed
ok
-1
-1
ok
-1
```

## ��ʾ
û��д����ʾ
## ��Ŀ��Դ
by AwD & HFLSyzx


