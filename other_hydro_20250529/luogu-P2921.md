## ��Ŀ����
Every year in Wisconsin the cows celebrate the USA autumn holiday of Halloween by dressing up in costumes and collecting candy that Farmer John leaves in the N (1 <= N <= 100,000) stalls conveniently numbered 1..N.

Because the barn is not so large, FJ makes sure the cows extend their fun by specifying a traversal route the cows must follow.  To implement this scheme for traveling back and forth through the barn, FJ has posted a 'next stall number' next\_i (1 <= next\_i <= N) on stall i that tells the cows which stall to visit next; the cows thus might travel the length of the barn many times in order to collect their candy.

FJ mandates that cow i should start collecting candy at stall i. A cow stops her candy collection if she arrives back at any stall she has already visited.

Calculate the number of unique stalls each cow visits before being forced to stop her candy collection.

POINTS: 100

## �����ʽ
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 contains a single integer: next\_i


## �����ʽ
\* Lines 1..N: Line i contains a single integer that is the total number of unique stalls visited by cow i before she returns to a stall  she has previously visited.


## ��Ŀ����
#### ��Ŀ����

ÿ�꣬����˹�����ݣ���ţ�Ƕ��ᴩ���·����ռ�ũ��Լ���� $N(1\le N\le 100,000)$ ��ţ����������µ��ǹ����Դ�����ף�����������ʥ�ڡ�

����ţ�ﲻ̫��FJ ͨ��ָ����ţ������ѭ�Ĵ�Խ·����ȷ����ţ����Ȥ��Ϊ��ʵ���������ţ��ţ�������ش���ķ�����FJ �ڵ� $i$ �Ÿ�����������һ�� ����һ�����䣺$next_i(1\le next_i\le N)$�� �ı��������ţҪȥ����һ�����䡣������Ϊ���ռ����ǵ��ǹ�����ţ�ͻ���ţ�������ش����ˡ�

FJ ������ţ $i$ Ӧ�ô� $i$ �Ÿ��俪ʼ�ռ��ǹ������һֻ��ţ�ص�ĳһ�����Ѿ�ȥ���ĸ��䣬���ͻ�ֹͣ�ռ��ǹ���

�ڱ���ֹͣ�ռ��ǹ�֮ǰ������һ��ÿͷ��ţҪǰ���ĸ�������������㣩��

#### �����ʽ

��һ��һ������ $n$����ʾţ������������

�� $2$ �� $n+1$ �У�ÿ�а���һ������ $next_i$����ʾ $i$ �Ÿ������һ�����䡣

#### �����ʽ

����� $n$ �У��� $i$ �а���һ����������ʾ�� $i$ ֻ��ţҪǰ���ĸ�������

#### ��������

�� $4$ �����䡣

- ���� $1$ Ҫ��ţ������ $1$��

- ���� $2$ Ҫ��ţ������ $3$��

- ���� $3$ Ҫ��ţ������ $2$��

- ���� $4$ Ҫ��ţ������ $3$��

ţ $1$���� $1\rightarrow 1$���ܹ����� $1$ �����䣻

ţ $2$��$2\rightarrow 3\rightarrow 2$���ܹ����� $2$ �����䣻

ţ $3$��$3\rightarrow 2\rightarrow 3$���ܹ����� $2$ �����䣻

ţ $4$��$4\rightarrow 3\rightarrow 2\rightarrow 3$���ܹ����� $3$ �����䡣

�����ṩ�ߣ�[busy_programmer](https://www.luogu.com.cn/user/649315)��

```input1
4 
1 
3 
2 
3 

```

```output1
1 
2 
2 
3 

```

## ��ʾ
Four stalls.

\* Stall 1 directs the cow back to stall 1.

\* Stall 2 directs the cow to stall 3

\* Stall 3 directs the cow to stall 2

\* Stall 4 directs the cow to stall 3


Cow 1:  Start at 1, next is 1.  Total stalls visited: 1.

Cow 2:  Start at 2, next is 3, next is 2.  Total stalls visited: 2. Cow 3:  Start at 3, next is 2, next is 3.  Total stalls visited: 2. Cow 4:  Start at 4, next is 3, next is 2, next is 3. Total stalls visited: 3.


