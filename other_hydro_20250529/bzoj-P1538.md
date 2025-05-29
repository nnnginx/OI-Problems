## ��Ŀ����

King Byteasar has decided to throw two great parties and wants to invite to them every single Byteotian inhabitant. Of course he wants to invite each of them to exactly one of the parties. The king knows from his own vast experience that a person is having a good time when there is an even number of her/his friends at the party. Thus he has asked you to divide the country's inhabitants between two parties in a way that as many people as possible have an even number of friends at their party. A trivial division, i.e. one that leaves one party with no guests invited, is allowed. The acquaintanceship is a symmetric relation, i.e. whenever a person $A$ knows the person $B$, the person $B$ also knows the person $A$.

��ռͥ����Ҫ�ٰ��������ɶԣ�����ϣ���������ľ��񣬹��������ķḻ������֪�������һ���������ɶ���������ż���������ѣ�������ǳ����ˡ���ˣ���Ҫ����������ҵľ���ȥ�����ɶԣ�ע������˵�Ѿ���ֵ������ɶ��ϣ�����ʹ�����ܶ���������ǵľۻ�����ż���������ѣ�����һС������û�вμ��ɶԡ���ʶ��һ�ֶԳƹ�ϵ���� $A$ ��ʶ $B$����ô $B$ Ҳ��ʶ $A$��

TaskWrite a programme that:

reads from the standard input the number of Byteotia's inhabitants and the description of their acquaintances,splits the inhabitants into two parties in such way that the number of people who have an even number of friends at their party is as large as possible,writes to the standard output a list of people who should be invited to the first party.

��������Ǳ�дһ������

�ӱ�׼�������ж�ȡ����������͸�����������ѣ��Ѿ��񻮷��������ɶԣ����Ҿ���ʹһ���������ɶ��ϵ�����������

## �����ʽ

In the first line of the standard input there is one integer $N$ ($1\le N\le 200$) - it is the number of inhabitants of Byteotia. The inhabitants are numbered from $1$ to $N$. In the following $N$ lines there are the descriptions of subsequent persons' acquaintances. At the beginning of the $(i+1)$'th line there is an integer $l_i$ ($0\le l_i\le N-1$) - the number of friends of the ith inhabitant. It is followed by $l_i$ pairwise distinct numbers of the $i$'th inhabitant's friends. We assume that no inhabitant is her/his own friend. It follows that each acquaintance is written twice: if $A$ and $B$ know each other, then $B$ appears on $A$'s list of friends and $A$ appears on $B$'s.

���빲 $N+1$ ���ڵ�һ�ж���һ������ $N$ - ��ʾ����������������� $N$ �У��� $i+1$ ����һ������ $l_i$����ʾ�� $i$ ����������������������� $l_i$ ������Ϊ�� $i$ ����������ѱ�š����Ǽ���û�������Լ������ѡ���� $B$ �������� $A$ �������б��У���ô $A$ Ҳ������� $B$ �������б��С�

## �����ʽ

In the first line of the standard output your programme should write one integer $M$ - the number of people who are to come to the first party. In the second line the $M$ numbers of these people should be written. The rest shall come to the second party.

There are many correct divisions in this task - your programme should write any one of them.

��һ����һ������ $M$����ǰ����һ���Ŷӵ��������ڶ��� $M$ ����������ȥ��һ���ɶԵľ����ţ�����ľ���ǰ���ڶ����ɶԡ�

�кܶ��ִ𰸣���ֻ��Ҫ���һ����

## ��������
```plain
5
3 2 3 4
2 1 3
4 2 1 4 5
2 1 3
1 3
```

## �������
```plain
3
1 2 3
```

## ���ݹ�ģ��Լ��

����  $100 \%$ ������ ��$1\le N\le 200$��
