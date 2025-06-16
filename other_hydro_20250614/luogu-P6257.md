## ��Ŀ����
### Warning: If you submit a malicious program, you will be banned.
### ���棺�����ύ���⽫����š�


## ��Ŀ����
In the Royal Family, names are very important! As the Royal Historian you have been charged with analyzing the patterns in the names of the Royal Ladies in the realm.

There have been n Royal Ladies, for convenience numbered from 1 to $n$. The name of each Lady is anuppercase letter concatenated with the name of her mother. The exception is the Lady numbered 1, the
founder of the Royal Family, whose name is just a single uppercase letter.

For example, ENERYS could be the mother of AENERYS (as the name AENERYS consists of the single uppercase letter 'A' concatenated with ENERYS, which is her mother's name). Similarly, AENERYS could be the mother of DAENERYS and YAENERYS.

You are given the description of all the Royal Ladies. Your task is to determine, for certain interesting strings $s$, the number of Royal Ladies for whom s is a prefix of their name.

For example, consider Sample Input 1 below, with a Royal Line that goes straight from the founder S to AENERYS (through YS, RYS, ERYS, NERYS and ENERYS), with each Lady having exactly one daughter. Then AENERYS has two daughters��DAENERYS and YAENERYS, with the latter havingone daughter, RYAENERYS.

In such a family, RY is a prefix of the names of two ladies: RYS and RYAENERYS. E is a prefix of the names of ERYS and ENERYS. N is a prefix only of NERYS's name, while S is a prefix only of the nameof the founder, S. AY is not a prefix of any Royal Lady's name.


## �����ʽ
The first line of input contains two integers $n$ and $k$, where $n$ $(1 \leq n \leq 10^6)$ is the total number of Royal Ladies and $k$ $(1 \leq k \leq 10^6)$ is the number of query strings.

Then follow n lines describing the Royal Ladies. The $i^{th}$ of these lines describes the Royal Lady numbered $i$, and contains an uppercase letter $c_i$ ('A'�C'Z') and an integer $p_i$, where $c_i$ is the first letter of the name of Lady $i$, and $p_i$ $(p1 = 0$ and $1 \leq pi \lt i$ for $i \gt 1)$ is the number of her mother (or $0$, in the case
of the First Lady). All the names are unique.

The remaining $k$ lines each contain one nonempty query string, consisting only of uppercase letters. The sum of the lengths of the query strings is at most $10^6$.

## �����ʽ
Output $k$ lines, with the $i^{th}$ line containing the number of Royal Ladies who have the $i^{th}$ query string as a prefix of their name.

## ��Ŀ����
**��Ŀ����**

������֪�����Ҽ�������ַǳ��н���������Ϊ�о����ҵ���ʷѧ�ҵ��㣬����ӵ���һ����޵����񡪡�����������ʷ�����л��ҷ��˵����֡�

������ʷ���� $n$ λ���ҷ��ˣ�������������ǽ���� $1$ �� $n$ ��š����� $1$ �ŷ����⣬������˵����־�Ϊһ����д��ĸ��������ĸ�׵����֡��� $1$ �ŷ�����Ϊ����������������������ֻ��һ����д��ĸ��

���磬���� `AENERYS` �� `A` �� `ENERYS` ��ɣ���� `ENERYS` �� `AENERYS` ��ĸ�ס����Ƶأ�`AENERYS` �� `DAENERYS` �� `YAENERYS` ��ĸ�ס�

��֪��������ʷ�����л��ҷ��˵��������ϵ��������Ҫ��ɵ������ǣ�����������ʷѧ�Ҹ���Ȥ�����ִ� $s$���ܹ��ж���λ���˵��������� $s$ ��ʼ�ġ�

�����������Ļ��������У�`S` �� `AENERYS` ����һ֧������ `YS`��`RYS`��`ERYS`��`NERYS` �� `ENERYS` �⼸λ���ˣ���ֻ��һλŮ���������� `AENERYS` ����λŮ�����ֱ��� `DAENERYS`���Լ�Ů���� `RYAENERYS` �� `YAENERYS`��

��������Ҽ����ڣ�����λ���˵������� `RY` ��ʼ�������� `RYS` �� `RYAENERYS`���� `ERYS` �� `ENERYS` ���� `E` ��ʼ�������� `N` ��ʼ�Ľ���һλ���� `NERYS`��ͬ���أ��� `S` ��ʼ�Ľ�����λ���� `S`����û���κ�һλ���˵������� `AY` ��ʼ��

**�����ʽ**

��һ������������ $n,k$���ֱ����������ʷ�ϻ��ҷ����������Լ�������ʷѧ�Ҹ���Ȥ�����ִ��ĸ�����

������ $n$ ���������л��ҷ��˵��������ϵ���� $i+1$ �������� $i$ λ���˵����� $c_i$ �� $p_i$�������ַ� $c_i$ ��ʾ�����ֵ���λ��ĸ��$p_i$ Ϊ��ĸ�׵ı�š����ڱ��Ϊ $1$ ����λ����$p_1=0$�����з��˵����־����ظ���

������ $k$ �У�ÿ��Ϊһ����д��ĸ���ɵķǿմ�������һ��������ʷѧ�Ҹ���Ȥ�����ִ���

**�����ʽ**

��� $k$ �У��� $i$ ��Ϊһ�������������ܹ��ж���λ���˵��������Ե� $i$ ������Ȥ�����ִ���ʼ�ġ�

**���ݷ�Χ**

$1\leq n\leq 10^6$��$1\leq k\leq 10^6$��$p_1=0$���ر�أ����� $1\lt i\leq n$����֤�� $1\leq p_i\lt i$������Ȥ�����ִ��ܳ������� $10^6$��

```input1
10 5
S 0
Y 1
R 2
E 3
N 4
E 5
A 6
D 7
Y 7
R 9
RY
E
N
S
AY
```

```output1
2
2
1
1
0
```

## ��ʾ
Source: ICPC World Finals 2019.

