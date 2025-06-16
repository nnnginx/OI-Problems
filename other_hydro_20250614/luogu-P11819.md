## ��Ŀ����
���� PA 2019 Final��


��������Ϊ���졣

std: zimpha��validator: Starrykiller��generator��KanameMadoka&Starrykiller��Special Thanks to @N_z_��

## ��Ŀ����


��һ�� $n$ ���ڵ�ļ������Ȩͼ��Radewoosh ��Ҫ�������ͼ��ȫԴ���·��������д�� Floyd-Warshall��

$$
\def\arraystretch{1.2}
    \begin{array}{ll}
    \hline
    \textbf{�㷨 1} & \text{\textbf{��ȷ��} Floyd-Warshall �㷨} \\
    \hline
    1&\textbf{Require: } n\times n \text{ �ľ��� }M�����㣺\\
    & M_{i,j}=\begin{cases}
                  0, & \text{�� } i=j \\
                  w_{i,j}, & \text{������һ�� } u\to v \text{ ������ߣ���ȨΪ } w_{i,j} \\
                  \infty, & \text{�������}
               \end{cases}
    \\
    2&\ \textbf{for } x=1,2,3,\ldots,n \textbf{ do} \\
    3&\ \qquad\textbf{for } y=1,2,3,\ldots,n \textbf{ do} \\
    4&\ \qquad\qquad\textbf{for } z=1,2,3,\ldots,n \textbf{ do} \\
    5&\ \qquad\qquad\qquad M_{y,z}\gets \min(M_{y,z},M_{y,x}+M_{x,z}) \\
    \hline
    \end{array} 
$$

Ȼ���������ѭ��˳�����Ǵ�������������

$$
\def\arraystretch{1.2}
    \begin{array}{ll}
    \hline
    \textbf{�㷨 2} & \text{\textbf{����ȷ��} Floyd-Warshall �㷨} \\
    \hline
    1&\textbf{Require: } n\times n \text{ �ľ��� }M�����㣺\\
    & M_{i,j}=\begin{cases}
                  0, & \text{�� } i=j \\
                  w_{i,j}, & \text{������һ�� } u\to v \text{ ������ߣ���ȨΪ } w_{i,j} \\
                  \infty, & \text{�������}
               \end{cases}
    \\
    2&\ \textbf{for } y=1,2,3,\ldots,n \textbf{ do} \\
    3&\ \qquad\textbf{for } z=1,2,3,\ldots,n \textbf{ do} \\
    4&\ \qquad\qquad\textbf{for } x=1,2,3,\ldots,n \textbf{ do} \\
    5&\ \qquad\qquad\qquad M_{y,z}\gets \min(M_{y,z},M_{y,x}+M_{x,z}) \\
    \hline
    \end{array} 
$$

������ͼ�У�$x\to y$ ��ȷ�ľ���Ϊ $\operatorname{dist}(x,y)$��Radewoosh �����Ϊ $\operatorname{dist}'(x,y)$��

������� $\operatorname{dist}(x,y)\neq \operatorname{dist}'(x,y)$ �� $(x,y)$ ������




## �����ʽ
��һ�У����������� $n,m$��

������ $m$ �У�ÿ������������ $u,v,w$����ʾһ����ȨΪ $w$ �� $u\to v$ ������ߡ�

## �����ʽ
���һ��һ���Ǹ���������ʾ�𰸡�


```input1
4 5
2 3 4
3 4 3
4 2 2
1 3 1
1 2 9
```

```output1
1
```

## ��ʾ
- $2\le n\le 2\times 10^3$��
- $1\le m\le 3\times 10^3$��
- $1\le u,v\le n$��$u\neq v$��
- $1\le w\le 10^5$��
- ������ͼ�Ǽ�ͼ�����ر��Ի�����

�������ͣ�

������ߵľ�������ȷ�� $\operatorname{dist}$ �����ұ��Ǵ���� $\operatorname{dist'}$ ����

$$\begin{bmatrix}0&6&1&4\\\infin&0&4&7\\\infin&5&0&3\\\infin&2&6&0\end{bmatrix}\qquad\begin{bmatrix}0&9&1&4\\\infin&0&4&7\\\infin&5&0&3\\\infin&2&6&0\end{bmatrix}$$

