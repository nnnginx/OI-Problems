## ��Ŀ����
Alice and Bob are playing a board game. The board is divided into positions labeled $a, b, c, d, \dots $ and the players use a gamepiece to mark the current position. Each round of the game consists of two steps:

Alice makes a choice. Depending on the current position, she has different options, where each option is a set of positions. Alice chooses one set $S$ among the available sets of positions.

Bob makes a choice. His choice is one position $p$ from the set $S$ that Alice chose in step 1. Bob moves the gamepiece to position $p$, which is the position for the start of the next round.

Prior to the first round, each player independently selects one of the positions and reveals it at the start of the game. Bob��s position is where the game starts. Alice wins the game if she can force Bob to move the gamepiece to the position she has chosen. To make things interesting, they have decided that Bob will pay Alice a certain amount if he loses, but Alice must pay Bob a certain amount after every round. The game now ends if Alice��s position is reached or when Alice runs out of cash.

Both Alice and Bob play optimally: Alice will always choose an option that will lead to her winning the game, if this is possible, and Bob will always try to prevent Alice from winning.

For all possible start and end positions, Alice would like you to determine whether she can win the game and if so, how many rounds it will take.

## �����ʽ
The input consists of a single test case. The first line contains the number of positions $n$ ($1 \leq n \leq 25$). The $n$ positions are labeled using the first $n$ letters of the English alphabet in lowercase. The rest of the test case consists of $n$ lines, one for each position $p$, in alphabetical order. The line for position $p$ contains the options available to Alice in position $p$. It starts with the number of options $m$ ($1 \leq m < 2^ n$), which is followed by $m$ distinct strings, one for each option. Each string contains the positions available to Bob if Alice chooses that option. The string has at least $1$ character, the characters (which correspond to valid board positions) are in alphabetical order, and no characters are duplicated. The total number of options for the test case is at most $10^6$.

## �����ʽ
For each position $p$ in alphabetical order, display one line. In that line, for each position $q$ in alphabetical order display the minimal number of rounds in which Alice can be guaranteed to arrive at position $q$ when starting the game in position $p$, or $-1$ if Alice cannot be guaranteed to reach $q$ from $p$.

## ��Ŀ����
### **��Ŀ����**

Alice �� Bob ������һ��������Ϸ�����̱��ֳ��˱��� $a,b,c,d,...$ ��λ�ã������ʹ����Ϸ��������ǵ�ǰλ�á���Ϸ��ÿһ�ְ����������裺

Alice �ж������ݵ�ǰλ�ã����в�ͬ��ѡ��ÿ��ѡ����һ��λ�á�Alice ���ӿ��õ�λ�ü�����ѡ��һ������ $S$��

Bob �ж�������ѡ���Ǽ��� $S$ �е�һ��λ�� $p$��Bob ����Ϸ�����ƶ���λ�� $p$���������һ����Ϸ����ʼλ�á�

�ڵ�һ��֮ǰ��ÿ����Ҷ���ѡ��һ��λ�ò�����Ϸ��ʼʱ����λ�á�Bob ��λ������Ϸ��ʼ�ĵط������ Alice �ܹ���ʹ Bob ����Ϸ�����ƶ�����ѡ���λ�ã�Alice ��Ӯ���˱�����Ϊ��ʹ�������Ȥ�����Ǿ������ Bob ���ˣ�����֧���� Alice һ������ Alice ������ÿ��֮���� Bob ֧��һ������� Bob ���� Alice ��λ�û��� Alice ûǮ�ˣ���Ϸ�ͽ����ˡ�Alice �� Bob ����ȡ��Ѳ��ԣ�������ܵĻ���Alice ����ѡ���������Ӯ�ñ����ķ������� Bob ������ͼ��ֹ Alice ��ʤ���������п��ܵ���ʼ�ͽ���λ�ã�Alice ϣ����ȷ�����Ƿ��ܹ�Ӯ�ñ�����������ԣ���Ҫ�����ֲ���Ӯ�ñ�����

### **�����ʽ**

�����ɵ���������ɡ���һ�а���λ���� $n$ $(1\le n\le 25)$����Щλ����Ӣ��Сд��ĸ��ǰ $n$ ����ĸ��ǡ������� $n$ �У�ÿ�б�ʾλ�� $p$������ĸ˳�����С�λ�� $p$ ��һ�а��� $Alice$ �ڸ�λ�õĿ�ѡ�ÿ����������һ���� $m$ $(1 \le m < 2^n)$����� $m$ ����ͬ�ַ�����ÿ���ַ�����ʾ Alice ѡ��÷���ʱ Bob ���ƶ�����λ�á��ַ������ٰ��� $1$ ���ַ�����Щ�ַ�����Ӧ��Ч������λ�ã�����ĸ˳�����У�û���ظ��ַ������ݵķ����������Ϊ $10^6$��

### **�����ʽ**

����ÿһ�� $p$ �������һ�С��ڸ����У�����ĸ˳�����ÿ��λ�� $q$ ��ʾ Alice ��ʼ��Ϸʱ���Ա�֤�������С�ִΣ�������� Alice ���ܱ�֤�� $p$ ���� $q$������ʾ $-1$��

### **˵��/��ʾ**

ʱ�����ƣ� $5000$ ms���ռ����ƣ�$1048576$ kB��

��Դ��International Collegiate Programming Contest (ACM-ICPC) World Finals 2014

```input1
2
2 ab b
1 b

```

```output1
0 1 
-1 0

```

```input2
3
1 b
2 b a
2 ab ac

```

```output2
0 1 -1 
1 0 -1 
2 2 0

```

## ��ʾ
Time limit: 5000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2014

