## ��Ŀ����
FJ's cows would like to be able to compute integer powers P (1 <= P <= 20,000) of numbers very quickly, but need your help. Because they're going to be computing powers of very large numbers, they can only keep around two work variables for intermediate results.

The first of those work variables is initialized to the number (denoted x) for which they are calculating the power; the other is initialized to 1. The cows can both multiply and divide any pair of the work variables and store the result in any work variable, but all results are stored as integers.

For example, if they want to compute x^31, one way to perform the calculation is:

![](https://cdn.luogu.com.cn/upload/image_hosting/bfbznh12.png)

Thus, x^31 can computed in six operations. Given the power to be computed and the the number of work variables, find the minimum number of operations to calculate the power.

## �����ʽ
A single line with one integer: P.

## �����ʽ
A single line with a single integer that is the minimum number of operations it requires to compute the pow

## ��Ŀ����
**����Ŀ������**

FJ ����ţ��ϣ���ܹ����ټ��������� $P$��$1 \leq P \leq 20000$������������Ҫ��İ�������Ϊ���ǽ�Ҫ����ǳ���������ݣ���������ֻ�ܱ������������������洢�м�����

���������������еĵ�һ������ʼ��Ϊ���ڼ����ݵ����֣���ʾΪ $x$������һ������ʼ��Ϊ $1$����ţ�ǿ��Զ�����һ�Թ����������г˷��ͳ������㣬��������洢������һ�����������У������н�����洢Ϊ������

���磬���������Ҫ���� $x^{31}$��һ�ֽ��м���ķ����ǣ�

![](https://cdn.luogu.com.cn/upload/image_hosting/bfbznh12.png)

��ˣ�$x^{31}$ ���������β����м������������Ҫ������ݺ͹����������������ҳ����������������ٲ�������

**�������ʽ��**

һ�У�һ��������$P$��

**�������ʽ��**

һ�У�һ����������ʾ�������������С��������

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
31
```

```output1
6
```

