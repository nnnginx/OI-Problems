


## ��Ŀ����
If you are an average football fan, you probably know that obtaining tickets for this year��s World Cup in Germany was an impossible task. Greedy organizers and football federations grabbed the majority or available tickets and divided them among sponsors, friends and family members. As a result, jet setters have flooded the venues, while die-hard fans sit at home enjoying the games between advertisements featuring crappy beer and sugar-free chewing gum. A couple of tickets are left for the final game and a huge queue has formed in front of the ticker office. As fans were arriving, they were labeled with successive integers. The first person in queue was labeled with number one, the second with number two, etc. Since the fans arrived the night before, they had to wait for a long time before the ticket counter was open and, naturally, some of them had to use the restroom. Each time a person needs to use the restroom, he/she steps out of the queue and, and, after completing the task, steps back into the queue, though not necessarily at the same position as before. Since there is only one restroom available no person leaves the queue before the previous person has returned (hence, at any moment there is at most one person missing from the queue). During the course of the night, a total of N restroom visits have occurred. Each visit is described by two positive integers A and B, denoting that the person labeled A stepped out of the queue and the stepped back into the queue immediately in front of the person labeled B. Now that all the visits have completed, the officials have to answer a series of questions. Each question is either of the form ��P X��, asking for the position lf the person labeled X, or of the form ��L X��, asking for the label of the person at position X. The first person in queue is considered to be at position one, the second at position two, etc. Write a program that, given the description of the visits and a number of questions, answers all of the questions. һ��ʼ��һ���˰���Ŵ�1��ʼ˳�����У�Ȼ�����N�β�����ÿ�ν����ΪA�����ó������ڱ��ΪB����ǰ�棬���в������������Q�����⣬ѯ�ʱ��ΪX���˵�λ�ã�����ѯ����X��λ���ϵ��˵ı�š�
## �����ʽ
The first line of input contains an integer N(2 �� N �� 50 000)- the total number of restroom visits. Each of the following N lines contains two different integers A and B (1 �� A, B �� 109), describing one restroom visit. The nest line contains an integer Q (1 �� Q �� 50 000) �C the total number of questions. Each of the following Q lines contains a single character (either the uppercase letter ��P�� or the uppercase letter ��L��) and an integer X (1�� X ��109) , describing one question.
## �����ʽ
The output should consist of a total of Q lines. The ith line or output should contain a single integer R �C the answer to the ith question. If the corresponding question is of the form ��P Xi�� then R should be the final position of the person labeled Xi. If the corresponding question is of the form ��L Xi�� then R should be the label of the person at position Xi. Grading Partial credit is awarded for incorrect solutions that correctly answer all questions of one type. If all questions of the form ��P X�� are answered correctly or if all questions of the form ��L X�� are answered correctly, you will receive 50% of the corresponding test case. In order to receive partial credit, the output should be formatted according to the specifications. Therefore, even if you choose to answer only one type of questions, you should still produce output for all questions of the other type.

```input1
2
6 3
9 6
8
L 1
L 2
L 3
L 4
P 1
P 2
P 3
P 4
Output
1
2
9
6
1
2
5
6
Input
5
7 2
2 7
9 7
10 1
10005 9995
9
L 1
P 2
L 2
P 7
L 7
P 9
P 10
P 99999
P 100000

```
```output1
10
3
1
5
4
4
1
99999 
100000
```

## ��ʾ
û��д����ʾ
## ��Ŀ��Դ
û��д����Դ


