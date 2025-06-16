## ��Ŀ����
Every day each of Farmer John's N $(1 \le N \le 100,000)$ cows conveniently numbered $1..N$ move from the barn to her private pasture. The pastures are organized as a tree, with the barn being on pasture $1$. Exactly $N-1$ cow unidirectional paths connect the pastures; directly connected pastures have exactly one path. Path $i$ connects pastures $A_i$ and $B_i$ $(1 \le A_i \le N,1 \le B_i \le N)$.

Cow $i$ has a private pasture $P_i(1 \le P_i \le N)$. The barn's small door lets only one cow exit at a time; and the patient cows wait until their predecessor arrives at her private pasture. First cow $1$ exits and moves to pasture $P_1$. Then cow $2$ exits and goes to pasture $P_2$, and so on.

While cow $i$ walks to $P_i$ she might or might not pass through a pasture that already contains an eating cow. When a cow is present in a pasture, cow $i$ walks slower than usual to prevent annoying her friend.

```cpp
Consider the following pasture network, where the number between
parentheses indicates the pastures' owner.

        1 (3)        
       / \
  (1) 4   3 (5)
     / \   
(2) 2   5 (4)

First, cow 1 walks to her pasture:

        1 (3)        
       / \
  [1] 4*  3 (5)
     / \   
(2) 2   5 (4)

When cow 2 moves to her pasture, she first passes into the barn's
pasture, pasture 1. Then she sneaks around cow 1 in pasture 4 before
arriving at her own pasture.

        1 (3)
       / \
  [1] 4*  3 (5)
     / \   
[2] 2*  5 (4)

Cow 3 doesn't get far at all -- she lounges in the barn's pasture, #1.

        1* [3]
       / \
  [1] 4*  3 (5)
     / \   
[2] 2*  5 (4)

Cow 4 must slow for pasture 1 and 4 on her way to pasture 5:

        1* [3]
       / \
  [1] 4*  3 (5)
     / \   
[2] 2*  5* [4]

Cow 5 slows for cow 3 in pasture 1 and then enters her own private pasture:

        1* [3]
       / \
  [1] 4*  3*[5]
     / \   
[2] 2*  5* [4]
```

FJ would like to know how many times each cow has to slow down.

ÿ�� Farmer John �� $N$ ͷ��ţ����� $1 \ldots N$�����������������Լ�������������������һ������������ $1$ ��������ǡ���� $N-1$ ����·ֱ��������������ʹ������֮�䶼ǡ����һ��·���������� $i$ ��·������ $A_i$ �� $B_i$����ţ��ÿ����һ��˽������ $P_i$�����ֵ���ÿ��ֻ����һֻ��ţ�뿪�����ĵ���ţ�ǻ�ȵ����ǵ�ǰ��������ǵ������Լ���˽����������뿪��������ţ $1$ �뿪��ǰ�� $P_1$��Ȼ������ţ $2$���Դ����ơ�

����ţ $i$ �������� $P_i$ ��ʱ�������ܻᾭ�����ڳԲݵ�ͬ���ԡ���·���Ѿ�����ţ������ʱ����ţ $i$ ������Լ����ٶȣ���ֹ�����������ѡ�

FJ ��Ҫ֪����ţ���ܹ�Ҫ�������ٴ��ٶȡ�

## �����ʽ

\* Line $1$: Line $1$ contains a single integer: $N$

\* Lines $2..N$: Line $i+1$ contains two space-separated integers: $A_i$ and $B_i$

\* Lines $N+1..N+N$: line $N+i$ contains a single integer: $P_i$

��һ�У���һ������ $N$��

�� $2 \sim N$ �У��� $i+1$ ���������Կո���������� $A_i$ �� $B_i$��

�� $N+1 \sim N+N$ �У��� $N+i$ ����һ������ $P_i$��

## �����ʽ
\* Lines $1 \sim N$��Line $i$ contains the number of times cow $i$ has to slow down.

�� $1 \sim N$ �У��� $i$ �а�����ţ $i$ ��Ҫ�����ٶȵĴ�����

```input1
5 
1 4 
5 4 
1 3 
2 4 
4 
2 
1 
5 
3 

```

```output1
0 
1 
0 
2 
1 

```

## ��ʾ
���ݷ�Χ��$1 \leq A_i,B_i,P_i\leq N \leq 10^5$��

