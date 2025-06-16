## ��Ŀ����
After many weeks of hard work, Bessie is finally getting a vacation! After many weeks of hard work, Bessie is finally getting a vacation!  numbered 1..N. The cows have set up quite an unusual road network with exactly N-1 roads connecting pairs of cows C1 and C2 (1 <= C1 <= N; 1 <= C2 <= N; C1 != C2) in such a way that there exists a unique path of roads between any two cows.

FJ wants Bessie to come back to the farm soon; thus, he has instructed Bessie that if two cows are directly connected by a road, she may not visit them both. Of course, Bessie would like her vacation to be as long as possible, so she would like to determine the maximum number of cows she can visit.

�����˼��ܵ����๤��,��������ӭ����һ������.��Ϊ��ţȺ������罻��ţ,��ϣ��ȥ�ݷ�N(1<=N<=50000)������.��Щ���ѱ����Ϊ1..N.��Щ��ţ��һ����ͬѰ���Ľ�ͨϵͳ,������N-1��·,ÿ��·������һ�Ա��ΪC1��C2����ţ(1 <= C1 <= N; 1 <= C2 <= N; C1<>C2).����,��ÿһ����ţ֮�䶼��һ��Ψһ��ͨ·. FJϣ�����羡��Ļص�ũ��.����,����ָʾ����,�������һ��·ֱ��������������ţ,����ֻ�ܰݷ����е�һ��.��Ȼ,����ϣ�����ļ���Խ��Խ��,��������֪�������԰ݷõ���ţ�������Ŀ.


## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N: Each line describes a single road with two

space-separated integers: C1 and C2


## �����ʽ
\* Line 1: A single integer representing the maximum number of cows that Bessie can visit.


```input1
7 
6 2 
3 4 
2 3 
1 2 
7 6 
5 6 

```

```output1
4 

```

## ��ʾ
Bessie knows 7 cows. Cows 6 and 2 are directly connected by a road, as are cows 3 and 4, cows 2 and 3, etc. The illustration below depicts the roads that connect the cows:

1--2--3--4

|
5--6--7


Bessie can visit four cows. The best combinations include two cows on the top row and two on the bottom. She can't visit cow 6 since that would preclude visiting cows 5 and 7; thus she visits 5 and 7. She can also visit two cows on the top row: {1,3}, {1,4}, or {2,4}.


