## ��Ŀ����
Farmer John must deliver a package to Farmer Dan, and is preparing to make his journey. To keep the peace, he gives a tasty treat to every cow that he meets along his way and, of course, FJ is so frugal that he would like to encounter as few cows as possible.

ũ��Լ��������һ��������ũ�򵤣���׼��ȥ���С�Ϊ�˱��ֺ�ƽ���������ÿһͷ��������ţһЩ�Եģ���Ȼ��FJ�ܽڼ�������������������ٵ���ţ��

FJ has plotted a map of N (1 <= N <= 50,000) barns, connected by M (1 <= M <= 50,000) bi-directional cow paths, each with C\_i (0 <= C\_i <= 1,000) cows ambling along it. A cow path connects two distinct barns, A\_i and B\_i (1 <= A\_i <= N; 1 <= B\_i <= N; A\_i != B\_i). Two barns may be directly connected by more than one path. He is currently located at barn 1, and Farmer Dan is located at barn N.

FJ �Ѿ������� $N(1 \le N \le 50000)$ ���Ȳֵĵ�ͼ��ͨ�� $M(1 \le M \le 50000)$ ��˫��ţ����ÿ��˫��ţ������ $c[i](0 \le c[i] \le 1000)$ ��ţ������˫��ţ������������ͬ�ĹȲ֣�$a[i]$ �� $b[i](1 \le a[i] \le N,1 \le b[i] \le N, a[i] \neq b[i])$�������Ȳֿ�����һ�����ϵ�С·ֱ�����ӡ���Ŀǰ�� $1$ �ŹȲ֣�ũ��λ�� $N$ �ŹȲ֡�

Consider the following map:

```cpp
           [2]---
          / |    \
         /1 |     \ 6
        /   |      \
     [1]   0|    --[3]
        \   |   /     \2
        4\  |  /4      [6]
          \ | /       /1
           [4]-----[5] 
                3  
```
The best path for Farmer John to take is to go from 1 -> 2 -> 4 -> 5 -> 6, because it will cost him 1 + 0 + 3 + 1 = 5 treats.

Given FJ's map, what is the minimal number of treats that he should bring with him, given that he will feed each distinct cow he meets exactly one treat? He does not care about the length of his journey.


## �����ʽ
\* Line 1: Two space-separated integers: N and M

\* Lines 2..M+1: Three space-separated integers: A\_i, B\_i, and C\_i


## �����ʽ
\* Line 1: The minimum number of treats that FJ must bring


```input1
6 8 
4 5 3 
2 4 0 
4 1 4 
2 1 1 
5 6 1 
3 6 2 
3 2 6 
3 4 4 

```

```output1
5 

```

