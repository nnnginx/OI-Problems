## ��Ŀ����


Brenda enjoys a new role-playing game Buffcraft. Shields, swords, books and other carry-on items do not affects character stats in Buffcraft. The only way to increase the stats of your character is to buff her.

There are two types of buffs in Buffcraft. Direct buffs increase a base value of the stat, while percentage buffs increase stats by the fraction of the base value. To be precise, if unbuffed base value of your character stat is $b$ , you have buffed her using $n$ direct buffs of strength $d_1 , d_2 , \cdots d_n$ and $m$ percentage buffs of strength $p_{1}, p_{2}, \cdots , p_{m},$ the resulting stat will be equal to $(b + d_{1} + d_{2} + �� �� �� + d_{n})(100 + p_{1} + p_{2} + �� �� �� + p_{m})/100$ . Note that the resulting stat may be fractional.

Unfortunately, your character has only $k$ buff slots and if you apply more than $k$ buffs on her, only the last $k$ buffs remains active. Thus, there is no reason to apply more than $k$ buffs simultaneously. You cannot apply the same buff more than once.

Brenda is going to send his character to raid and wants to buff her health to maximal possible value. She has some direct and some percentage buffs at her disposal and needs your help to select the set of buffs that leads to maximal possible total health.



## �����ʽ


The first line of the input file contains four integers $b , k , c_{d}$ and $c_{p}$ �� the base health of the character, the number of buff slots, the number of available directs buffs, and the number of available percentage buffs.

The following line contains $c_{d}$ integers $d_{i}$ �� strengths of direct buffs.

The last line of the input file contains $c_{p}$ integer numbers $p_{i}$ �� strengths of percentage buffs.

All numbers in the input file are greater than or equal to zero, and less than or equal to fifty thousand.



## �����ʽ


The first line of the output file must contain two integers $n$ and $m$ �� the number of direct and percentage buffs to use $(0 \le n \le c_{d}; 0 \le m \le c_{p}; 0 \le n + m \le k)$ .

The following line must contain $n$ different numbers �� indices of direct buffs to apply (buffs are numbered from one).

The last line of the output must contain $m$ different numbers �� indices of percentage buffs to apply (also numbered from one).

The resulting total health after application of all $n + m$ buffs must be maximal possible.



## ��Ŀ����
## ��Ŀ���� 
Brendaϲ��һ���µ���ϷBuffcraft��û���κ���Ʒ����Ӱ��Buffcraft�еĽ�ɫ���ԡ��������ɫ���Ե�Ψһ�������Ǹ�����buff��

Buffcraft�����������͵�buff��  
1.ֱ������buff��ֵ;  
2.�ٷֱ�����buff��ֵ;  
�����Ľ�ɫbuff��ʼֵ��$b$����ô��ʹ��$n$������ֱ�Ϊ$d_1,d_2,\cdots,d_n$�ĵ�һ��buff��$m$������ֱ�Ϊ$p_{1},p_{2}\cdots,p_{m}$�ĵڶ���buff���õ��Ľ��������$(b+d_{1}+d_{2}+����+d_{n})(100+p_{1}+p_{2}-����+p_{m})/100$����ע�⣬���������ܲ���������

���ҵ��ǣ���Ľ�ɫֻ��$k$��buff�ۣ��������������Ӧ����$k$�����ϵ�buff����ôֻ������$k$��buff��Ч����ˣ��㲻��ͬʱӵ��$k$������buff����Ȼ��һ��buff���ܱ����ʹ�á�

Brenda�������Ľ�ɫȥս������ϣ������ɫ��buffֵ�����������һЩ��һ��buff��һЩ�ڶ���buff�ɹ���ʹ�á�����Ҫ��İ�����ѡ��һ��buff�Ĵ��䷽ʽ���Ի�������ܵ���buffֵ��

## �����ʽ 
��һ�а����ĸ�����$b,k,n,m$���ֱ�����ɫ�Ļ���buffֵ��buff��������һ��buff��������ڶ���buff��������     
�ڶ��а���$n$������$d_{i}$������ÿ����һ��buff����������   
�����а���$m$������$p_{i}$������ÿ���ڶ���buff����������

## �����ʽ
��һ������������$x,y$�������˶��ٵ�һ��buff�����˶��ٵڶ���buff��$(0 \le x \le n; 0 \le y \le m; 0 \le x + y \le k)$ .
  
�ڶ�����$x$������-ҪӦ�õ�ÿһ����һ��buff��������  
�ڶ�����$y$������-ҪӦ�õ�ÿһ���ڶ���buff��������
��ķ���Ҫ������buffӦ�ú��������buffֵ���������

## �����������

### ��������#1
```
70 3 2 2
40 30
50 40
```
### �������#1
```
2 1
2 1
1
```
### ��������#2
```
1 2 3 4
6 6 5
8 10 7 9
```
### �������#2
```
2 0
1 2
```
## ˵��/��ʾ
$0 \le b,k,n,m,d_{i},p_{i} \le 50000$  
�����������1��ʼ  
ʱ������:2s;�ռ�����:256MB��

```input1
70 3 2 2
40 30
50 40

```

```output1
2 1
2 1
1

```

```input2
1 2 3 4
6 6 5
8 10 7 9

```

```output2
2 0
1 2

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



