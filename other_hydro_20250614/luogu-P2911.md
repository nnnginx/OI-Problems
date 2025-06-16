## ��Ŀ����
Bessie loves board games and role-playing games so she persuaded Farmer John to drive her to the hobby shop where she purchased three dice for rolling. These fair dice have S1, S2, and S3 sides

respectively (2 <= S1 <= 20; 2 <= S2 <= 20; 2 <= S3 <= 40). 

Bessie rolls and rolls and rolls trying to figure out which three-dice sum appears most often.

Given the number of sides on each of the three dice, determine which three-dice sum appears most frequently. If more than one sum can appear most frequently, report the smallest such sum.

POINTS: 70


## �����ʽ
\* Line 1: Three space-separated integers: S1, S2, and S3


## �����ʽ
\* Line 1: The smallest integer sum that appears most frequently when the dice are rolled in every possible combination.


## ��Ŀ����
����ϲ����������Ϸ�ͽ�ɫ������Ϸ��������˵����Լ����������ȥС�̵�.�������������������ӡ���������ͬ�����ӵ������ֱ�Ϊ $s_1,s_2,s_3$��

����һ���� $S$ ���������ÿ�����ϵ������� $1,2,3,\ldots,S$��ÿ���棨�ϵ����֣����ֵĸ��ʾ��ȡ�����ϣ���ҳ������С��������ϵ����ֵĺ͡��У��ĸ��͵�ֵ���ֵĸ������

���ڸ���ÿ�����ӵ���������Ҫ����ĸ����С��������ϵ����ֵĺ͡����ֵ���Ƶ��������кܶ���ͳ��ֵĸ�����ͬ����ôֻ��Ҫ�����С���Ǹ���

���ݷ�Χ�� $2\le s_1\leq 20$��$2 \leq s_2\leq 20$��$2 \leq s_3\leq 40$��

```input1
3 2 3 

```

```output1
5 

```

## ��ʾ
Here are all the possible outcomes.

```
1 1 1 -> 3  
1 2 1 -> 4  
2 1 1 -> 4  
2 2 1 -> 5  
3 1 1 -> 5  
3 2 1 -> 6 
1 1 2 -> 4  
1 2 2 -> 5  
2 1 2 -> 5  
2 2 2 -> 6  
3 1 2 -> 6  
3 2 2 -> 7 
1 1 3 -> 5  
1 2 3 -> 6  
2 1 3 -> 6  
2 2 3 -> 7  
3 1 3 -> 7  
3 2 3 -> 8
```
Both 5 and 6 appear most frequently (five times each), so 5 is the answer.


