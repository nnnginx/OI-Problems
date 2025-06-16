## ��Ŀ����
This past fall, Farmer John took the cows to visit a corn maze. But this wasn't just any corn maze: it featured several gravity-powered teleporter slides, which cause cows to teleport instantly from one point in the maze to another. The slides work in both directions: a cow can slide from the slide's start to the end instantly, or from the end to the start. If a cow steps on a space that hosts either end of a slide, she must use the slide.

The outside of the corn maze is entirely corn except for a single exit.

The maze can be represented by an N x M (2 <= N <= 300; 2 <= M <= 300) grid. Each grid element contains one of these items:

\* Corn (corn grid elements are impassable) 

\* Grass (easy to pass through!) 

\* A slide endpoint (which will transport a cow to the other endpoint) 

\* The exit

A cow can only move from one space to the next if they are adjacent and neither contains corn. Each grassy space has four potential neighbors to which a cow can travel. It takes 1 unit of time to move from a grassy space to an adjacent space; it takes 0 units of time to move from one slide endpoint to the other.

Corn-filled spaces are denoted with an octothorpe (#). Grassy spaces are denoted with a period (.). Pairs of slide endpoints are denoted with the same uppercase letter (A-Z), and no two different slides have endpoints denoted with the same letter. The exit is denoted with the equals sign (=).

Bessie got lost. She knows where she is on the grid, and marked her current grassy space with the 'at' symbol (@). What is the minimum time she needs to move to the exit space?


## �����ʽ
��һ�У������ÿո���������� $N$ �� $M$��

�� $2\sim N+1$ �У��� $i+1$ ���������Թ��еĵ� $i$ �е����������$M$���ַ���ÿ���ַ��м�û�пո񣩡�

## �����ʽ
һ����������ʾ��㵽������������ʱ�䡣

## ��Ŀ����
��ţ��ȥһ�� $N\times M$ �����Թ���$2 \leq N \leq 300,2 \leq M \leq300$��

�Թ�����һЩ����װ�ã����Խ���ţ��һ�㵽��һ�����˲��ת�ơ���Щװ�ÿ���˫��ʹ�á�

���һͷ��ţ�������װ�õ��������յ㣬��ͷ��ţ�ͱ���ʹ�����װ�ã���ţ�ڴ��͹��󲻻����̽��еڶ��δ��ͣ������Ῠ�ڴ���װ�õ������յ�֮�����ش��͡�

�����Թ�����Ψһ��һ�����ڶ������װ�Χ��

�Թ��е�ÿ��Ԫ�ض���������Ŀ�е�һ����ɣ�

1. ���ף�`#` ��ʾ����Щ�����ǲ�����ͨ���ġ�
1. �ݵأ�`.` ��ʾ�����Լ򵥵�ͨ����
1. ����װ�ã�ÿһ�Դ�д��ĸ $\tt{A}$ �� $\tt{Z}$ ��ʾ��
1. ���ڣ�`=` ��ʾ��
1. ��㣬 `@` ��ʾ

��ţ����һ��ݵ��Ͽ��ܴ��ڵ��ĸ����ڵĸ����ƶ������� $1$ ����λʱ�䡣��װ�õ�һ����㵽��һ����㲻��ʱ�䡣

```input1
5 6
###=##
#.W.##
#.####
#.@W##
######

```

```output1
3
```

## ��ʾ
�������¾���$N=5,M=6$��

```plain
###=##
#.W.##
#.####
#.@W##
######
```

Ψһ��һ��װ�õĽ���ô�д��ĸ $\tt{W}$ ��ʾ��

���ŷ���Ϊ���������ߵ�װ�õĽ�㣬����һ����λʱ�䣬�ٵ�װ�õ���һ������ϣ����� $0$ ����λʱ�䣬Ȼ����������һ������������һ����������ڴ����ܹ������� $3$ ����λʱ�䡣

