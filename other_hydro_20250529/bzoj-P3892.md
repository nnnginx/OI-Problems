## ��Ŀ����

Unhappy with the poor health of his cows, Farmer John enrolls them in an assortment of different physical fitness activities. His prize cow Bessie is enrolled in a running class, where she is eventually expected to run a marathon through the downtown area of the city near Farmer John's farm! The marathon course consists of $n$ checkpoints to be visited in sequence, where checkpoint $1$ is the starting location and checkpoint $n$ is the finish. Bessie is supposed to visit all of these checkpoints one by one, but being the lazy cow she is, she decides that she will skip up to $k$ checkpoints in order to shorten her total journey. She cannot skip checkpoints $1$ or $n$, however, since that would be too noticeable. Please help Bessie find the minimum distance that she has to run if she can skip up to $k$ checkpoints. Since the course is set in a downtown area with a grid of streets, the distance between two checkpoints at locations $(x_1, y_1)$ and $(x_2,y_2)$ is given by $\left|x1-x2\right|+\left|y1-y2\right|$.

�ڶ�άƽ������ $n$ ���㣬�� $(x_1, y_1)$ �� $(x_2,y_2)$ �Ĵ���Ϊ $\left|x1-x2\right|+\left|y1-y2\right|$��

��� $1$ �ŵ���������� $1$ �� $n$ ��˳�����ε���ÿ�������С�ܴ��ۡ�

���� $k$ �λ����������ĳ���㣬���������� $1$ �ŵ�� $n$ �ŵ㡣

## �����ʽ

The first line gives the values of $n$ and $k$. The next $n$ lines each contain two space-separated integers, $x_i$ and $y_i$, representing a checkpoint. The checkpoints are given in the order that they must be visited. Note that the course might cross over itself several times, with several checkpoints occurring at the same physical location. When Bessie skips such a checkpoint, she only skips one instance of the checkpoint -- she does not skip every checkpoint occurring at the same location.

## �����ʽ

Output the minimum distance that Bessie can run by skipping up to $k$ checkpoints.

```input1
5 2
0 0
8 3
1 1
10 -5
2 2

```

```output1
4
```

## ����˵��

In the sample case shown here, skipping the checkpoints at $(8, 3)$ and $(10, -5)$ leads to the minimum total distance of $4$.

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$3 \le n \le 500$��$k<n$��$-10^3 \le x_i,y_i \le 10^3$��

## ��Ŀ��Դ

Silver