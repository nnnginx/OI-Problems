## ��Ŀ����
A full moon casts some sort of spell on the cows and, like their cousins the wolves and coyotes, they bay at the moon -- mooing instead of howling, of course.

Each 'moo' lasts a certain amount of time. A short 'moo' might last time 1; a longer one might last time 24 or even 1,000,000,000 or longer (cows can really moo when they want to). No 'moo' will last more than or equal to 2^63.

It should come as no surprise that the cows have a pattern to their moos.  Bessie will choose an integer c (1 <= c <= 100) that is the initial length of a moo.

After Bessie moos for length c, the cows calculate times for

subsequent moos. They apply two formulae to each moo time to yield even more moo times. The two formulae are:

```cpp
f1(c)=a1*c/d1+b1 (integer divide, of course) and 
f2(c)=a2*c/d2+b2. 
They then successively use the two new times created by evaluating f1(c) and f2(c) to create even more mooing times. They keep a sorted list of all the possible mooing times (discarding duplicates). 
They are allowed to moo a total of N times (1 <= N <= 4,000,000). Please determine the length of the longest moo before they must quit. 
The constants in the formulae have these constraints: 1 <= d1 < a1; d1 < a1 <= 20; 0 <= b1 <= 20; 1 <= d2 < a2; d2 < a2 <= 20; 0 <= b2 <= 20. 
Consider an example where c=3 and N=10. The constants are: 
a1=4    b1=3     d1=3 
a2=17   b2=8     d2=2 
```
The first mooing time is 3, given by the value of c. The total list of mooing times is:
```cpp
1. c=3             ->  3       6. f2(3)=17*3/2+8  -> 33 
2. f1(3)=4*3/3+3   ->  7       7. f1(28)=4*28/3+3 -> 40 
3. f1(7)=4*7/3+3   -> 12       8. f1(33)=4*33/3+3 -> 47 
4. f1(12)=4*12/3+3 -> 19       9. f1(40)=4*40/3+3 -> 56 
5. f1(19)=4*19/3+3 -> 28      10. f1(47)=4*47/3+3 -> 65 
The tenth time is 65, which would be the proper answer for this set of inputs. 
```
Partial feedback will be provided on the first 50 submissions.
MEMORY LIMIT: 64MB

���µ�ʱ�򣬺���һ����ţ��Ҳ���¹��½У����ǴӲ����У�������С�

ÿ����ж���һ��ʱ���������� $1$ �룬������ $10^9$ �����ã�ţ����ķǳ��ܽ�.��Ȼ��û�����ʱ���ᳬ������� $2^{63}$��

ţ�ǵ���п����ҵ����ɣ��Ⲣ����֡������ѡ��һ������ $c(c\le100)$ ����Ϊ��ʼʱ��֮��ţ�Ǹ���������ʽȷ�������ʱ����

$f_1(c)=\lfloor a_1c/d_1\rfloor+b_1$

$f_2(c)=\lfloor a_2c/d_2\rfloor+b_2$ 

ţ������������ʽ���ϵص��������㣬��ô�����ʱ��.Ȼ�����ǽ���Щʱ�������޳��ظ���ʱ�������ȡǰ $N(1<N< 4000000)$ ������Ϊ���� $N$ ����е�ʱ��.������㣬�� $N$ ����е�ʱ���Ƕ��١���ʽ�еĳ�����Ϊ�������������й�ϵ�� 

$1 \le d_1 < a_1 \le 20$; $0\le b_1 \le 20$;

$1 \le d_2 < a_2 \le 20$; $0\le b_2\le 20$��


## �����ʽ
\* Line 1: Two space-separated integers: c and N

\* Line 2: Three space-separated integers: a1, b1, and d1

\* Line 3: Three space-separated integers: a2, b2, and d2


## �����ʽ
\* Line 1: A single line which contains a single integer which is the length of the Nth moo


```input1
3 10 
4 3 3 
17 8 2 

```

```output1
65 

```

