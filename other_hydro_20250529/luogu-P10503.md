## ��Ŀ����
In our daily life we often use 233 to express our feelings. Actually, we may say 2333, 23333, or 233333 ... in the same meaning. And here is the question: Suppose we have a matrix called 233 matrix. In the first line, it would be 233, 2333, 23333... (it means $a _ {0,1} = 233$, $a_{0,2} = 2333$, $a_{0,3} = 23333$...) Besides, in 233 matrix, we got $a_{i,j} = a_{i-1,j} +a_{i,j-1}( i,j \neq 0)$. Now you have known $a_{1,0},a_{2,0},\dots,a_{n,0}$, could you tell me $a_{n,m}$ in the 233 matrix?

## �����ʽ
There are multiple test cases. Please process till EOF.

For each case, the first line contains two postive integers $n,m(n \le 10,m \le 10^9)$. The second line contains n integers, $a_{1,0},a_{2,0},...,a_{n,0}$ ($0 \le a_i,0 < 2^{31}$).

## �����ʽ
For each case, output $a_{n,m}$ mod 10000007.

## ��Ŀ����
**����Ŀ������**

�����ǵ��ճ������У����Ǿ����� 233 ��������ǵ���С�ʵ���ϣ����ǿ��ܻ�˵ 2333��23333 ���� 233333... ����ʾͬ������˼��������һ�����⣺����������һ����Ϊ 233 �����ڵ�һ�У��������� 233��2333��23333...����ʾ $a _ {0,1} = 233$��$a_{0,2} = 2333$��$a_{0,3} = 23333$...�������⣬�� 233 �����У������� $a_{i,j} = a_{i-1,j} +a_{i,j-1}( i,j \neq 0)$��������֪ $a_{1,0},a_{2,0},\dots,a_{n,0}$�����ܸ����� 233 �����е� $a_{n,m}$ ��

**�������ʽ��**

�ж�������������봦��ֱ�� EOF��

����ÿ����������һ�а������������� $n,m(n \le 10,m \le 10^9)$���ڶ��а��� n ��������$a_{1,0},a_{2,0},...,a_{n,0}$��$0 \le a_i,0 < 2^{31}$����

**�������ʽ��**

����ÿ����������� $a_{n,m}$ ģ 10000007��

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
1 1
1
2 2
0 0
3 7
23 47 16
```

```output1
234
2799
72937
```

## ��ʾ
![](https://cdn.luogu.com.cn/upload/image_hosting/ndjcn0l1.png)

