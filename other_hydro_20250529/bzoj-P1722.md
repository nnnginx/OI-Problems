## ��Ŀ����
Farmer John's $n \ (1 \le  n \le  500)$ cows are trying to select the milking team for the world-famous Multistate Milking Match-up (MMM) competition. As you probably know, any team that produces at least $x \ (1 \le  x \le  10^6)$ gallons of milk is a winner. Each cow has the potential of contributing between $-10^4$ and $10^4$ gallons of milk.(Sadly, some cows have a tendency to knock over jugs containing milk produced by other cows.) The MMM prides itself on promoting family values. FJ's cows have no doubt that they can produce $x$ gallons of milk and win the contest, but to support the contest's spirit, they want to send a team with as many parent-child relationships as possible (while still producing at least $x$ gallons of milk). Not surprisingly, all the cows on FJ's farm are female. Given the family tree of FJ's cows and the amount of milk that each would contribute, compute the maximum number of parent-child relationships that can exist in a winning team. Note that a set of cows with a grandmother-mother-daughter combination has two parent-child relationships (grandmother-mother, mother-daughter).


Լ���� $n$ ͷ��ţ�������ȥ�μ�һ�����缶�Ĳ��̱��� MultistateMilking Match-up������дΪ MMM�������Ǻ���������ӵ�ʵ����Ҳ����˵�������ɳ��Ķ�ֻҪ�ܲ������� $x$ ����ţ�̣�����Ӯ���ⳡ������ÿͷţ����Ϊ���幱��һ������ţ�̣���ֵ�� $-10^4$ �� $10^4$ ֮�䣨��Щ��ţ������Ū��װ��������ţ�����̵�ƿ�ӣ���MMM �ľٰ�Ŀ��֮һ����ͨ�������еĺ�����������ͥ��Ա֮���Ĭ������ţ����Ϊ����������Ӯ���ⳡ��������Ϊ�˱�ʾ�Ա��������֧�֣�����ϣ����ѡ���Ķ��������о����ܶ��ţ����ͬһ����ͥ��Ҳ����˵���о����ܶ�Ե�ţ��ֱϵѪԵ��ϵ����Ȼ����֧��������ܲ������� $x$ ����ţ�̣�����Ȼ�ˣ����е���ţ����Ů�ԣ����Զ���������ֱϵѪ�׶���ĸŮ��ϵ��Լ����֪������ţ֮���ѪԵ��ϵ����������֪��������ڱ�֤һ֧������Ӯ�ñ���������£�����������ܴ��ڶ��ٶ�ѪԵ��ϵ��ע�⣬���һ֧������ĳͷ��ţ������ĸ�ס���������ĸ��ɣ�����֧������һ���� $2$ ��ѪԵ��ϵ����ͷ��ţ����ĸ������ĸ�ף��Լ���������ĸ�ף���
## �����ʽ
* Line $1$: Two space-separated integers,$n$ and $x$.
* Lines $2\dots n+1$: Line $i+1$ contains two space-separated integers describing cow $i$. The first integer is the number of gallons of milk cow $i$ would contribute. The second integer (range $1\dots n$) is the index of the cow's mother. If the cow's mother is unknown, the second number is $0$. The family information has no cycles: no cow is her own mother, grandmother, etc.

- ��һ�У������ÿո���������� $n$ �� $x$��
- �ڶ��� $n+1$ �У�ÿ�а��������ÿո��������������һ����Ϊһֻ��ţ�ܹ��׳���ţ�̵ļ��������ڶ�������ʾ����ĸ�׵ı�š��������ĸ�ײ�������ţȺ��ǵڶ�����Ϊ $0$�����ң�ѪԵ��Ϣ�������ѭ����Ҳ����˵һͷ��ţ�������Լ���ĸ�׻���ĸ�����߸��ߴ������ȡ�

## �����ʽ
* Line $1$: The maximum number of parent-child relationships possible on a winning team. Print `-1` if no team can win.

* �����һ���ܻ�ʤ�Ķ����У������ܴ��ڵ���ѪԵ��ϵ��ţ�Ķ���������κ�һ֧���鶼�����ܻ�ʤ����� `-1`��
```input1
5 8
-1 0
3 1
5 1
-3 3
2 0
```
```output1
2
```
## ����˵��

INPUT DETAILS��  
There are $5$ cows. Cow $1$ can produce $-1$ gallons and has two daughters, cow $2$ and $3$, who can produce $3$ and $5$ gallons, respectively. Cow $3$ has a daughter (cow $4$) who can produce $-3$ gallons. Then there's cow $5$, who can produce $2$ gallons.

Լ��һ���� $5$ ͷ��ţ���� $1$ ͷ��ţ���ṩ $-1$ ���ص�ţ�̣������ǵ� $2$���� $3$ ͷ��ţ��ĸ�ס��� $2$���� $3$ ͷ��ţ�Ĳ��������Ϊ $3$ ���غ� $5$ ���ء��� $4$ ͷ��ţ�ǵ� $3$ ͷ��ţ��Ů���������ṩ $-3$ ����ţ�̡�����������ţ��û�й�ϵ�ĵ� $5$ ͷ��ţ�����Ĳ������� $2$ ���ء���õ�һ֧��������� $1,2,3,5$ ͷ��ţ������һ���ܲ��� $\ (-1)+3+5+2=9��8$ ����ţ�̣�������֧�������� $2$ ��ţ��ѪԵ��ϵ��$1��2$ �� $1-3$�������ֻѡ�� $2,3,5$ ͷ��ţ����Ȼ�ܲ���������ߣ�$10$ ���أ�������֧�����������ѪԵ��ϵ�Ķ�������һ������٣�������û��ѪԵ��ϵ�ԣ���

## ���ݹ�ģ��Լ��
���� $100\%$ �����ݣ�$1 \leq n \leq 500$��$1 \leq x \leq 10^6$��
## ��Ŀ��Դ
Gold