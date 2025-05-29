## ��Ŀ����
Bessie wants to navigate her spaceship through a dangerous asteroid field in the shape of an $n \times n$ grid $\ (1 \le  n \le  500)$. The grid contains $k$ asteroids $\ (1 \le  k \le  10^4)$, which are conveniently located at the lattice points of the grid. Fortunately, Bessie has a powerful weapon that can vaporize all the asteroids in any given row or column of the grid with a single shot. This weapon is quite expensive, so she wishes to use it sparingly. Given the location of all the asteroids in the field, find the minimum number of shots Bessie needs to fire to eliminate all of the asteroids.

�������ʻ���ķɴ�����Σ�յ�С����Ⱥ��С����Ⱥ��һ�� $n\times n$ ���������������� $k$ ��С���ǡ����˵��Ǳ�����һ����ǿ���������һ�ο�������������һ�л�һ���е�С���ǣ����������ܹ�������ϣ�����������á��������е�С���ǵ�λ�ã��������������Ҫ���ٴ���������������е�С���ǡ�
## �����ʽ
* Line $1$: Two integers $n$ and $k$, separated by a single space.
* Lines $2\dots k+1$: Each line contains two space-separated integers $r$ and $c \ (1 \le  r, c \le  n)$ denoting the row and column coordinates of an asteroid, respectively.
* ��һ�У��������� $n$ �� $k$����һ���ո������
* �ڶ����� $k+1$ �У�ÿһ���������ո���������� $r,c$���ֱ��ʾС�������ڵ��к��С�
## �����ʽ
* Line $1$: The integer representing the minimum number of times Bessie must shoot.
* һ��������ʾ������Ҫ��������������������������е�С���ǡ�
```input1
3 4
1 1
1 3
2 2
3 2
```
```output1
2
```
## ����˵��
INPUT DETAILS:  
The following diagram represents the data, where `X` is an asteroid and `.` is empty space:  
```
X.X
.X.
.X.
```
OUTPUT DETAILS:  
Bessie may fire across row $1$ to destroy the asteroids at $(1,1)$ and$(1,3)$, and then she may fire down column $2$ to destroy the asteroids at $(2,2)$ and $(3,2)$.

## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq n \leq 500$��$1 \leq k \leq 10^4$��$1 \leq r,c \leq n$��
## ��Ŀ��Դ
Gold