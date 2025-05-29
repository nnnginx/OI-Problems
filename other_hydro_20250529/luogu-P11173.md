## ��Ŀ����
![](bilibili:BV1qW4y1Q7Ce)

$\small\color{white}54^{\text{th}}\text{Problem by ArCu}.$

## ��Ŀ����
���� $n\times n$ ���� $A$������ $f(A)$ Ϊ��С������ $A^b=O$ �������� $b$�������������������� $f(A)=0$������ $O$ ������󣬼�����Ԫ�ض��� $0$ �ľ���

���� $n,a$��ÿ��Ԫ�ض��� $[0,a)$ �������� $n\times n$ ������ $a^{n^2}$ �֡������� $a^{n^2}$ �ֿ��ܵľ��� $A$ �� $f(A)$ ֮�͡�

�𰸶� $202407031$ ȡģ��

## �����ʽ
һ���������� $n,a(1\leq n\leq 600,0<a<2^{64})$��

## �����ʽ
һ��һ����������ʾ����õĴ𰸡�

```input1
2 2
```

```output1
5
```

```input2
3 4
```

```output2
793
```

```input3
5 10
```

```output3
59350891
```

```input4
18 15932416
```

```output4
52138206
```

```input5
1 1
```

```output5
1
```

## ��ʾ
$\text{Sample 1 Explanation}:$

ע�⵽�������������� $b$��$\begin{bmatrix}1&0\\1&1\end{bmatrix}^b\neq O$������ $f\left(\begin{bmatrix}1&0\\1&1\end{bmatrix}\right)=0$���� $\begin{bmatrix}0&0\\1&0\end{bmatrix}^2=O$������ $f\left(\begin{bmatrix}0&0\\1&0\end{bmatrix}\right)=2$��

һ���� $2^4=16$ �ֿ��ܵľ������� $f(A)$ ��Ϊ $0$ ��ֻ��

$$f\left(\begin{bmatrix}0&0\\0&0\end{bmatrix}\right)=1,f\left(\begin{bmatrix}0&0\\1&0\end{bmatrix}\right)=f\left(\begin{bmatrix}0&1\\0&0\end{bmatrix}\right)=2$$

�𰸼�Ϊ $1+2+2=5$��

$\text{Details of Subtasks}:$

������������ $1\leq n\leq 600,0<a<2^{64}$��

| $\text{Subtask}$ | $\text{Special Constraints}$ | $\text{Score}$ |
| :----------: | :----------: | :----------: | 
| $1$ | $n\leq 5,a\leq 2$ | $3$ |
| $2$ | $n\leq 5$ | $7$ | 
| $3$ | $n\leq 10$ | $10$ | 
| $4$ | $n\leq 40$ | $20$ | 
| $5$ | $n\leq 200$ | $30$ |
| $6$ |  | $30$ |

$\text{Hint}:202407031=13009\times 15559.$

