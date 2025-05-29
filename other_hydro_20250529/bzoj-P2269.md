## ��Ŀ����

A wizard is in a labyrinth where there are $V$ rooms and $V-1$ doors connecting some pairs of rooms in both directions��in such a way that there is always a sequence of doors one can traverse to go from a room to any other room��
Additionally��there are $C$ locks and $C$ keys of $C$ different colours��one of each��in some of the doors and rooms of the maze��respectively��each door has at most one lock��and there is at most one key placed in each room��It should be an easy matter for the wizard to bypass the lock system��were it not for the fact that he forgot his spell book��without which his wizardry is utterly useless��The wizard is currently in room $X$��and he wants to get his spell book��located in room $Y$��without taking too long��At every step he may go to an adjacent room through one of the doors��Of course��if the door is locked��he needs to be carrying the key of the same colour as the lock��unless��of course��that door has already been unlocked����The wizard can carry only one key at a time and after picking up a key it is not possible for him to drop it somewhere in the maze in order to take it again afterwards��Once a door has been unlocked��the key is thrown away since it is no longer any use��
Given the maze and the positions of the $C$ keys and $C$ locks��determine how to reach $Y$ from $X$��if possible��Any path whose length does not exceed $4 \times(C��1)\times V$ is acceptable��

һ����ʦĿǰ��������һ������ $V$ ������� $V-1$ ��������ĳЩ������ŵ��Թ����Ȼ���Ŷ��ǿ�˫��ͨ�еģ������ǿ��Դ�һ�����侭��һϵ�е��ŵ�����һ�����䡣��ĳЩ��������Կ�ף���ĳЩ����������

����Կ�׹��� $C$ ����ɫ��ÿһ����ɫ����Ӧ��Ψһ��Կ�׺�Ψһ������һ��Կ�׿��Կ���ͬ��ɫ������һ�����������һ������һ�������������һ��Կ�ס������ʦû�ж�ʧ�����飬������ʦ��ͬ���衣���ڣ���ʧ�����������ʦ����������һ��������

��ʦĿǰ�� $X$ �ŷ��䡣��ϣ������̫���ʱ��Ϳ����õ������� $Y$ ����������顣��һ�������ߵ����ڵķ��䡣��Ȼඣ������������������������Ϻ���ͬɫ��Կ�ף���������򿪾�û��Ҫ�ˣ�����ʦһ��ֻ�ܴ�һ��Կ�ף�����һ��������һ��Կ�ף��Ͳ��ܰ�������ض����Թ����ĳһ��λ�ò���֮���ĳһʱ���������ֻ�е�Կ�׿������Ժ���ܶ�������

�����Թ�����̬�� $C$ ��Կ�׺� $C$ ������λ�á�������Դ� $X$ �� $Y$��������������κ�һ�������� $4 \times(C + 1)\times V$ ���ķ������ǿ��Ա����ܵġ�

## �����ʽ

**�����ж�������**

The first line of each case contains four integers��the number $V$ of rooms in the maze ��the number $C$ of locks ��and rooms $X$ and $Y$ numbered $0,1,\dots ,V-1$��

Then comes a��possibly empty��line with $C$ integers indicating the location of each of the keys��in order of increasing colour��

The next $V-1$ lines describe the maze��each contains three integers $A,B,L$��meaning that there is a door between rooms $A$ and $B$ which can be unlocked with the key of colour $L$��if $0 \le L < C$ ��a value of $-1$ for $L$ indicates that no lock is needed��

The last line has $V,C,X,Y = 0,0,0,0$��

ÿһ���������ݵĵ�һ�а���4��������$V$ ��������, $C$ ������ɫ������ $X��Y$�����䱻���Ϊ $0��1 \dots V-1��

��������һ�а����� $C$ ��������ʾ $C$ ��Կ�׵�λ�ã�Կ�׵���ɫ�ǵ����ġ�

�������� $V-1$ ���������Թ�����̬��ÿһ�а������������� $A,B,L$����ʾ�ڷ��� $A$ �� $B$ ����һ��˫���ţ����Ϲ���һ����ɫΪ $L$ �������� $L = -1$ ����ʾ��û����

���һ��Ϊ $V,C,X,Y = 0,0,0,0$

## �����ʽ

**ÿһ���������ݶ�Ӧһ�������**

���û�н⣬��� `Impossible`������ $L:V_0 \dots V_L$ �ĸ�ʽ�����$L$ ���ܲ�����Ӧ���� $L \le 4 \times ��C + 1�� \times V$��

$X = V_0,V_1,\dots,V_{L-1}$��$V_L = Y$ ��һ�ξ����� $L + 1$ ���㡣����������Ӧ����һ���ո�ֿ���������μ�������

```input1
1 0 0 0
3 1 0 2
1
0 1 -1
0 2 0
3 2 0 2
1 2
0 1 1
0 2 0
5 3 0 4
2 0 3
0 1 0
0 2 -1
1 3 1
2 4 2
0 0 0 0
```

```output1
0: 0
3: 0 1 0 2
Impossible
10: 0 2 0 1 0 1 3 1 0 2 4
```

## ��Ŀ��Դ

��л������

## ���ݹ�ģ��Լ��

$100\%$ ���������㣺$1 \le V \le 1.5 \times 10^3$��$0 \le C < V$��