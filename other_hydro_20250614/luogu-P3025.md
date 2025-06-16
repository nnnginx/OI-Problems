## ��Ŀ����
As has happened to so many of us, Bessie has forgotten her cowtube password. She does, however, remember some handy bits of information about it.

First, she remembers that her password (denoted as variable P) has length L (1 <= L <= 1,000) roman characters and can be split into one or more words (not necessarily unique) from a dictionary composed of NW (1 <= NW <= 1,000) unique words.  A word W\_i is defined as a sequence of 1..20 lowercase letters of the Roman alphabet ('a'..'z').

She also remembers certain letters from her password along with their positions.

Consider the following example. Bessie knows that her password looks like 'a??l?ban???????' ('?' represents a letter she cannot remember), and her dictionary has the following words:

apple
cow
farmer
banana
bananas

pies
The two possible passwords for Bessie to have are 'applebananapies' and 'applebananascow'.

Given the dictionary, and the letters that Bessie remembers, please find her password. If more than one password is valid, find the lexicographically least string that works.

�������������Ϸ����ܶ�ε����һ����Bessie��һ������������ţ������Ա���룬��ֻ�ܼǵ������һ���֡�


���ȣ����ǵ����������ǳ���ΪL��1<=L<=1000�����ַ������������������г��ֹ������е��ʶ���¼������NW�����ʵ��ֵ��У��ֵ��еĵ���Wi����1-20����ĸ��ɵĵ��ʡ�


��ֻ�ǵ����������е�һ������ĸ������λ�á����磬Bessie�ǵ���������Ϊ��a??l?ban???????�������У����������ܼǵõ���ĸ���������ֵ��������������г��ֵ����е��ʡ�apple cow farmer banana bananas pies��������ע�⣬�ֵ��еĵ��ʿ��Բ��������г��ֵ������еĵ���һ�����ֵ��С����ԣ�Bessie����������ֿ����ǡ�applebananapies���͡�applebananascow������Ϊǰһ���ֵ����ǰ���������applebananapies����


���ڣ�����Bessie�ǵõ���ĸ�������ֵ䣬�����Ĺ���Ա���롣����ж���𰸣�������ֵ����С����һ����


## �����ʽ
\* Line 1: Two space-separated integers: L and NW

\* Line 2: A string of length L: P

\* Lines 3..NW+2: Line i+2 contains the ith word in the dictionary: W\_i

�� ��һ�У�������ĳ���L�͵�������NW����һ���ո����


�� �ڶ��У������ǵõ������ַ�����û�ж���ո�


�� �����е���NW+2�У�����Wi��һ��һ������


## �����ʽ
\* Line 1: The lexicographically least password that fits

һ�У�Bessie�����룬��Ҫ�ж���ո�


```input1
15 6 
a??l?ban??????? 
apple 
cow 
farmer 
banana 
bananas 
pies 

```

```output1
applebananapies 

```

## ��ʾ
��л@JJYZ\_cbh �ṩ����


