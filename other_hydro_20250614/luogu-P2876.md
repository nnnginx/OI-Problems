## ��Ŀ����
In easier times, Farmer John's cows had no problems. These days, though, they have problems, lots of problems; they have P (1 �� P �� 300) problems, to be exact. They have quit providing milk and have taken regular jobs like all other good citizens. In fact, on a normal month they make M (1 �� M �� 1000) money.

Their problems, however, are so complex they must hire consultants to solve them. Consultants are not free, but they are competent: consultants can solve any problem in a single month. Each consultant demands two payments: one in advance (1 �� payment �� M) to be paid at the start of the month problem-solving is commenced and one more payment at the start of the month after the problem is solved (1 �� payment �� M). Thus, each month the cows can spend the money earned during the previous month to pay for consultants. Cows are spendthrifts: they can never save any money from month-to-month; money not used is wasted on cow candy.

Since the problems to be solved depend on each other, they must be solved mostly in order. For example, problem 3 must be solved before problem 4 or during the same month as problem 4.

Determine the number of months it takes to solve all of the cows' problems and pay for the solutions.



## �����ʽ
Line 1: Two space-separated integers: M and P.


Lines 2..P+1: Line i+1 describes problem i with two space-separated integers: Bi and Ai. Bi is the payment to the consult BEFORE the problem is solved; Ai is the payment to the consult AFTER the problem is solved.



## �����ʽ
Line 1: The number of months it takes to solve and pay for all the cows' problems.


## ��Ŀ����
�ھ���״���Ϻõ�ʱ��FJ ����ţû���κ����⡣����������� $P$��$1 \le P \le 300$�������⡣���ǲ����ṩţ�̣����������������ù���һ���ҵ��˹̶��Ĺ�������ʵ�ϣ���һ���������·ݣ�����׬�� $M$��$1 \le M \le 1000$��ԪǮ�� 

Ȼ�������ǵ�����ǳ����ӣ����Ǳ���Ƹ��������������ѯʦ������ѵģ������Ǻ�����������ѯʦ������һ�����ڽ���κ����⡣ÿ����ѯʦҪ�����θ��һ�����ڿ�ʼ���������³���ǰ֧�� $a_i$ Ԫ��$1 \le a_i \le M$������һ����������������³���֧�� $b_i$ Ԫ��$1 \le b_i \le M$����������ţÿ���¾Ϳ������ϸ���׬��Ǯ��֧����ѯʦ�ķ��á�

������Ҫ������������໥����ģ��������Ǳ�������ϰ�˳���������磬���� $3$ ���������� $4$ ֮ǰ��������������� $4$ ��ͬһ�����ڽ���� 

ȷ�������ţ���������������������֧����������ķ��á�

ע�⣺��ţ�����Ǯ��ÿ����׬����Ǯû������ͻ���ʧ��

```input1
100 5
40 20
60 20
30 50
30 50
40 40
```

```output1
6
```

## ��ʾ
|      | Avail | Probs  | Before  | After   | Candy  |
| :-----------: | :-----------: | :-----------: | :-----------: | :-----------: | :-----------: |
|Month | Money | Solved | Payment | Payment | Money  |
| 1    | 0     | -none- | 0       | 0       | 0      |
| 2    | 100   | 1, 2   | 40+60   | 0       | 0      |
| 3    | 100   | 3, 4   | 30+30   | 20+20   | 0      |
| 4    | 100   | -none- | 0       | 50+50   | 0      |
| 5    | 100   | 5      | 40      | 0       | 60     |
| 6    | 100   | -none- | 0       | 40      | 60     |

