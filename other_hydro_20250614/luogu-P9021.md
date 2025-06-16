## ��Ŀ����
For the New Year celebration, Bessie and her friends have constructed a giant tree with many glowing ornaments. Bessie has the ability to turn the ornaments on and off through remote control. Before the sun rises, she wants to toggle some of the ornaments in some order (possibly toggling an ornament more than once) such that the tree starts and ends with no ornaments on. Bessie thinks the tree looks cool if the set of activated ornaments is exactly a subtree rooted at some vertex. She wants the order of ornaments she toggles to satisfy the property that, for every subtree, at some point in time it was exactly the set of all turned on ornaments. Additionally, it takes energy to switch on and off ornaments, and Bessie does not want to waste energy, so she wants to find the minimum number of toggles she can perform. 

Formally, you have a tree with vertices labeled $1 \cdots N (2 \le N \le 2 \cdot 10^5)$ rooted at $1$. Each vertex is initially inactive. In one operation, you can toggle the state of a single vertex from inactive to active or vice versa. Output the minimum possible length of a sequence of operations satisfying both of the following conditions: 

 - Define the subtree rooted at a vertex $r$ to consist of all vertices $v$ such that $r$ lies on the path from $1$ to $v$ inclusive. For every one of the $N$ subtrees of the tree, there is a moment in time when the set of active vertices is precisely those in that subtree. 
 - Every vertex is inactive after the entire sequence of operations.

## �����ʽ
The first line contains $N$.

The second line contains $p_2 \cdots p_N
(1 \le p_i<i)$, where $p_i$ denotes the parent of vertex $i$ in the tree. 

## �����ʽ
Output the minimum possible length. 

## ��Ŀ����
## ��Ŀ����

����һ�ø�Ϊ $1$ ������������Ϊ $1 \dots N$ $(2 \le N \le 2 \cdot 10^5)$ ��ÿ������������ǹرյġ���һ�β����У�����Խ�һ�������״̬�ӹر�״̬�л�������״̬����֮��Ȼ�����һ�������������������Ĳ������е���С���ܳ��ȡ�

- �����Զ��� $r$ Ϊ������������������ $r$ λ�ڴ� $1$ �� $v$ ��·���� $($���� $v)$ , �Ķ��� $v$ ��ɡ�ÿһ�����������������һ��ʱ�̣�����״̬����ļ���ǡ���Ǹ������еĶ��㡣
- ��������������֮��ÿ�����㶼�ǹرյġ�

## �����ʽ

��һ�а��� $N$ ��

�ڶ��а��� $p_2 \dots p_N$ �� $p_i$ �ǽ�� $i$ �ĸ��� $(1\le p_i < i)$ ��

## �����ʽ

������ܵ���С���ȡ�

## ��ʾ

�������������ֱ��Ӧ $\{1,2,3\}��\{2\}��\{3\}$ ����������С���ܳ��ȵ�һ���������С�

- ���� $2$ (����Ķ����γ��� $2$ Ϊ��������) ��
- ���� $1$ ��
- ���� $3$ (����Ķ����γ��� $1$ Ϊ��������) ��
- �ر� $1$ ��
- �ر� $2$ (����Ķ����γ��� $3$ Ϊ��������) ��
- �ر� $3$ ��

������
- ���Ե� $2-3$ : $N \le 8$
- ���Ե� $4-9$ : $N \le 40$
- ���Ե� $10-15$ : $N \le 5000$
- ���Ե� $16-21$ ��û�ж�������ơ�

```input1
3
1 1
```

```output1
6
```

## ��ʾ
### Explanation for Sample 1

There are three subtrees, corresponding to $\{1,2,3\}$, $\{2\}$, and $\{3\}$. Here is one sequence of operations of the minimum possible length:

activate 2  
(activated vertices form the subtree rooted at 2)  
activate 1  
activate 3  
(activated vertices form the subtree rooted at 1)  
deactivate 1  
deactivate 2  
(activated vertices form the subtree rooted at 3)  
deactivate 3

### Scoring

 - Inputs $2-3$: $N \le 8$
 - Inputs $4-9$: $N \le 40$
 - Inputs $10-15$: $N \le 5000$
 - Inputs $16-21$: No additional constraints.


