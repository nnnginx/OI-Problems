## ��Ŀ����
Farmer John's $N$ cows ($1 \leq N \leq 200$) want to organize an emergency"moo-cast" system for broadcasting important messages among themselves.


Instead of mooing at each-other over long distances, the cows decide to equip themselves with walkie-talkies, one for each cow.  These walkie-talkies each have a limited transmission radius -- a walkie-talkie of power $P$ can only transmit to other cows up to a distance of $P$ away (note that cow A might be able to transmit to cow B even if cow B cannot transmit back, due to cow A's power being larger than that of cow B).  Fortunately, cows can relay messages to one-another along a path consisting of several hops, so it is not necessary for every cow to be able to transmit directly to every other cow.


Due to the asymmetrical nature of the walkie-talkie transmission, broadcasts from some cows may be more effective than from other cows in their ability toreach large numbers of recipients (taking relaying into account).  Please  help the cows determine the maximum number of cows that can be reached by a broadcast originating from a single cow.







## �����ʽ
The first line of input contains $N$.


The next $N$ lines each contain the $x$ and $y$ coordinates of a single cow ( integers in the range $0 \ldots 25,000$) followed by $p$, the power of the walkie-talkie held by this cow.


## �����ʽ
Write a single line of output containing the maximum number of cows a broadcast from a single cow can reach.  The originating cow is included in this number.




## ��Ŀ����
### ��Ŀ����

Լ��ũ������ $N$ ͷ��ţ�뽨��һ����������µġ�����㲥��ϵͳ���������ǾͿ������Լ��м�㲥��Ҫ��Ϣ��

��ţ������ÿͷţװ����һ���Խ������������ڳ�����������һͷ��ţ�����衱�ҽС���Щ�Խ���ÿ̨���и��Ե���Ч����뾶����һ��ӵ�� $P$ �����ĶԽ���ֻ��������� $P$ ���ڵ�ţ������Ϣ��ע����ܳ��� $A$ ţ�Խ����������� $B$ ţ�Ĵ󣬶� $A$ ţ���Ը� $B$ ţ������Ϣ���� $B$ ţ���ܴ�����Ϣ�������˵��ǣ���ţ�ǿ���ͨ��������ţ�м̣�����һ����Ծ��·��������Ϣ�����ÿ����ţ����Ҫֱ����ÿ��������ţ������

���ڶԽ����ķѶѳ����ʣ�����һЩ��ţ�Ĺ㲥���ܱ�������ţ�Ĺ㲥�ܹ��ﵽ����Ľ����ߣ������м̵����������������Ч���������ţȷ�����Ե�����ţ�Ĺ㲥���Դﵽ����ţ�����������

### �����ʽ

��һ�У�һ������ $N$��

������ $N$ �У��� $i$ �а����� $i$ ֻţ������ $(x_i,y_i)$���Լ���ֻţ�����жԽ��������� $P_i$��

### �����ʽ

һ�У�һ����������ʾ�����Ե�����ţ�Ĺ㲥���Դﵽ����ţ�������������ʼ��ţҲ��������������С�

### ˵��/��ʾ

���� $100\%$ �����ݣ�$N\le200$��$\forall i \in [1,N]$��$0\le x_i,y_i\le25000$��

```input1
4
1 3 5
5 4 3
7 2 1
6 1 1
```

```output1
3
```

