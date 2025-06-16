## ��Ŀ����
**Note: The memory limit for this problem is 512MB, twice the default.**

Farmer John created $N(1 \le N \le 10^5)$ problems. He then recruited $M (1 \le M \le 20)$ test-solvers, each of which rated every problem as "easy" or "hard."

His goal is now to create a problemset arranged in increasing order of difficulty, consisting of some subset of his $N$ problems arranged in some order. There must exist no pair of problems such that some test-solver thinks the problem later in the order is easy but the problem earlier in the order is hard.

Count the number of distinct nonempty problemsets he can form, modulo $10^9+7$. 

## �����ʽ
The first line contains $N$ and $M$.

The next $M$ lines each contain a string of length $N$. The $i$-th character of this string is `E` if the test-solver thinks the ith problem is easy, or `H` otherwise. 

## �����ʽ
The number of distinct problemsets FJ can form, modulo $10^9+7$. 

## ��Ŀ����
Farmer John ���� $n$ ���⣬Ƹ�� $m$ ����������Ʒ���Ѷȡ�

�Ѷ�ֻ�м򵥣�`E`�������ѣ�`H`�����֡�

Farmer John ������ѡ�����ɵ���**����һ��**��������һ��˳�����У�ʹ��ǰһ����Ŀ������һ�����ô������ѵ�������Ҳ���ú���һ����Ŀ���ѡ�

�ش��ж�����ѡ���������еķ������� $10^9+7$ ȡģ��

$1\le n\le10^5$��$1\le m\le20$��

```input1
3 1
EHE
```

```output1
9
```

```input2
10 6
EHEEEHHEEH
EHHHEEHHHE
EHEHEHEEHH
HEHEEEHEEE
HHEEHEEEHE
EHHEEEEEHE
```

```output2
33
```

## ��ʾ
### Explanation for Sample 1

The nine possible problemsets are as follows:

$[1]$  
$[1,2]$  
$[1,3]$  
$[1,3,2]$  
$[2]$  
$[3]$  
$[3,1]$  
$[3,2]$  
$[3,1,2]$  

Note that the order of the problems within the problemset matters. 

### SCORING

 - Inputs $3-4$: $M=1$
 - Inputs $5-14$: $M \le 16$
 - Inputs $15-22$: No additional constraints.

