


## ��Ŀ����
Mr. Furion is a math teacher. His students are very lazy and they do not like to do their homework. One day, Mr. Furion decides to give them a special problem in order to see whether his students are talents in math or they are just too lazy to do their homework. The problem is: 
Given an integer k, n integers m_{1},m_{2}��m_{n}, and a formula below: 
X_{1} xor X_{2} xor X_{3}�� xor X_{n} = k 
Please figure out that how many integral solutions of the formula can satisfy: 
0<=X_{i}<=m_{i} (i=1��n)
������������K��N��һ����������M1,M2...Mn
������X1 Xor X2 Xor X3...Xor Xn=k��0<=Xi<=Mi��i=1...n)�Ľ�ĸ���
## �����ʽ
There are at most 100 test cases. 
The first line of each test case contains two integers, n and k. The second line of each test case contains n integers: m_{1},m_{2}��m_{n}. The meaning of n,k, m_{1},m_{2}��m_{n} are described above. (1<=n<=50,0<=k,m_{1},m_{2}��m_{n}<=2^{31}-1 ) 
The input is ended by ��0 0��
## �����ʽ
You should output an integer for each test case, which is the number of solutions. As the number might be very large, you should only output the number modulo 1000000003.

```input1
11 2047
1024 512 256 128 64 32 16 8 4 2 1
10 2047
1024 512 256 128 64 32 16 8 4 2 
0 0

```
```output1

1
0
```

## ��ʾ
û��д����ʾ
## ��Ŀ��Դ
û��д����Դ


