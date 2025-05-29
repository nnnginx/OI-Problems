## ��Ŀ����
For the new year, Farmer John decided to give his cows a festive binary search tree
(BST)! 

To generate the BST, FJ starts with a permutation $a=\{a_1,a_2,\ldots,a_N\}$
of the integers $1\ldots N$, where $N\le 300$.  He then runs the following
pseudocode with arguments $1$ and $N.$

```
generate(l,r):
  if l > r, return empty subtree;
  x = argmin_{l <= i <= r} a_i; // index of min a_i in {a_l,...,a_r}
  return a BST with x as the root, 
    generate(l,x-1) as the left subtree,
    generate(x+1,r) as the right subtree;
```
For example, the permutation $\{3,2,5,1,4\}$ generates the following BST:

```
    4
   / \
  2   5
 / \ 
1   3
```
Let $d_i(a)$ denote the depth of node $i$ in the tree corresponding to $a,$ 
meaning the number of nodes on the path from $a_i$ to the root. In the above
example, $d_4(a)=1, d_2(a)=d_5(a)=2,$ and $d_1(a)=d_3(a)=3.$

The number of inversions of $a$ is equal to the number of pairs of integers
$(i,j)$ such that $1\le i<j\le N$ and $a_i>a_j.$ The cows know that the $a$ that
FJ will use to generate the BST has exactly $K$ inversions
$(0\le K\le \frac{N(N-1)}{2})$.  Over all $a$ satisfying this condition, compute
the remainder when $\sum_ad_i(a)$ is divided by $M$ for each $1\le i\le N.$

## ��Ŀ����
Ϊ��ӭ�����꣬Farmer John ������������ţ��һ�����ն�����������

Ϊ���������������������Farmer John ��һ�� $1 \dots N$ ������ $a= \{1,2, \dots ,N\}$ ��ʼ��Ȼ���Բ��� $l$ �� $r$ ��ʼ�������µ�α���룺
```
generate(l,r):
  if l > r, return empty subtree;
  x = argmin_{l <= i <= r} a_i; // index of min a_i in {a_l,...,a_r}
  return a BST with x as the root, 
    generate(l,x-1) as the left subtree,
    generate(x+1,r) as the right subtree;
```
���磬���� $\{ 3,2,5,1,4 \}$ ���������µĶ�����������

![](https://cdn.luogu.com.cn/upload/image_hosting/gw6ursc0.png)

�� $d_i(a)$ ��ʾ�ڵ� $i$ �������� $a$ ���ɵĶ����������е���ȡ���ȶ���Ϊ����ڵ㵽���ڵ��·���ϵĵ����������������У�$d_4(a)=1,d_2(a)=d_5(a)=2,d_1(a)=d_3(a)=3$��

$a$ �е���������������� $1 \le i<j \le N$ �� $a_i>a_j$ ������ $(i,j)$ �ĸ�������ţ��֪�� Farmer John �������ɶ��������������� $a$ ��ǡ���� $K$ ������ԡ������������������� $a$����������ÿ�� $1 \le i \le N$��$\sum_a d_i(a)$ �� $M$ ȡģ��Ľ����

## �����ʽ
����ֻ��һ�У������������� $N,K,M$��

## �����ʽ
���һ�� $N$ ���������� $i$ ��������ʾ $\sum_a d_i(a) \bmod M$����������֮����һ���ո������

```input1
3 0 192603497

```

```output1
1 2 3

```

```input2
3 1 144408983

```

```output2
3 4 4

```

## ��ʾ
#### �������� 1

�������������Ψһ��������������Ϊ $a=\{1,2,3\}$��

#### �������� 2

������������������������������зֱ�Ϊ $a=\{1,3,2\}$ �� $a=\{2,1,3\}$��

#### ���ݷ�Χ

����ȫ�����ݣ�$1\le N\le 300$��$0\le K\le \frac{N(N-1)}{2}$����֤ $M$ ��һ�� $\left[ 10^8,10^9+9 \right]$ ��Χ�е�������

���ڲ��Ե� $3,4$������ $N \le 8$��

���ڲ��Ե� $5-7$������ $N \le 20$��

���ڲ��Ե� $8-10$������ $N \le 50$��

USACO 2019 December ������T3

