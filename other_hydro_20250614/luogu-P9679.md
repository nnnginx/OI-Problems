## ��Ŀ����
Prof. Pang is given $n$ numbers $a_1,\ldots, a_n$. It is easy to add the numbers up using a computer. But Prof. Pang treasures his computer so much and wants to reduce its workload. He decides to simulate the following program by hand. 

![](https://cdn.luogu.com.cn/upload/image_hosting/ajtj92in.png)


Unlike a computer, the time needed for Prof. Pang to simulate the program is proportional to the total number of **carries**(which means ����λ�� in Chinese) when calculating $s+a[i]$ for each $i$ from $1$ to $n$. Prof. Pang adds numbers **by column addition in base-ten**, just like what we normally do in primary school. For example, there are two carries in the following addition.

![](https://cdn.luogu.com.cn/upload/image_hosting/c779jeox.png)

Please permute the array $a_1,\ldots, a_n$ so that the total number of carries when Prof. Pang simulates the program is as small as possible. (By ''permute an array'', we mean that you can change the order of the elements arbitrarily.)


## �����ʽ
The first line contains one integer $T~(1\le T \le 10^5)$, the number of test cases.

For each test case, the first line contains one positive integer $n~(1\le n \le 10^5)$. The next line contains $n$ integers $a_1,\ldots, a_n~(1 \le a_i\le 10^9)$ denoting the numbers Prof. Pang is given. 

It is guaranteed that the sum of $n$ over all test cases is no more than $10^5$.

## �����ʽ
For each test case, output one line containing the minimum amount of carries.

## ��Ŀ����
### ��Ҫ����

�������Ƕ���һ���������� $a+b$ ���ٶ��� $a+b$ �г��ֵĽ�λ�Ĵ�����

����һ������ $a_1,a_2,...,a_n$�����ҳ���ȷ������ʹ�ü����������ĺ�ʱ���е��ٶ���̣����ҳ����ٵĽ�λ������

### �����ʽ

**�����ж�������**��

��һ��һ������ $T$����ʾ����������

����ÿ�����ݣ�

��һ��һ������ $n$��  

������һ�� $n$ ����������ʾ��������� $a$��

### �����ʽ

����ÿ�����ݣ������С�Ľ�λ������

### ���ݷ�Χ

���� $100 \%$ �����ݣ� $1 \leq \sum n \leq 10^5$�� $1 \leq a_i \leq 10^9$

```input1
2
3
9 99 999
1
12345
```

```output1
5
0
```

