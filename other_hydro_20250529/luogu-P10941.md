## 题目描述
A supermarket in Tehran is open 24 hours a day every day and needs a number of cashiers to fit its need. The supermarket manager has hired you to help him, solve his problem. The problem is that the supermarket needs different number of cashiers at different times of each day (for example, a few cashiers after midnight, and many in the afternoon) to provide good service to its customers, and he wants to hire the least number of cashiers for this job.

The manager has provided you with the least number of cashiers needed for every one-hour slot of the day. This data is given as R(0), R(1), ..., R(23): R(0) represents the least number of cashiers needed from midnight to 1:00 A.M., R(1) shows this number for duration of 1:00 A.M. to 2:00 A.M., and so on. Note that these numbers are the same every day. There are N qualified applicants for this job. Each applicant i works non-stop once each 24 hours in a shift of exactly 8 hours starting from a specified hour, say ti (0 <= ti <= 23), exactly from the start of the hour mentioned. That is, if the ith applicant is hired, he/she will work starting from ti o'clock sharp for 8 hours. Cashiers do not replace one another and work exactly as scheduled, and there are enough cash registers and counters for those who are hired.

You are to write a program to read the R(i) 's for i=0..23 and ti 's for i=1..N that are all, non-negative integer numbers and compute the least number of cashiers needed to be employed to meet the mentioned constraints. Note that there can be more cashiers than the least number needed for a specific slot.


## 输入格式
The first line of input is the number of test cases for this problem (at most 20). Each test case starts with 24 integer numbers representing the R(0), R(1), ..., R(23) in one line (R(i) can be at most 1000). Then there is N, number of applicants in another line (0 <= N <= 1000), after which come N lines each containing one ti (0 <= ti <= 23). There are no blank lines between test cases.


## 输出格式
For each test case, the output should be written in one line, which is the least number of cashiers needed. If there is no solution for the test case, you should write No Solution for that case.

## 题目大意
## 题目描述
翻译：

德黑兰的一家超市每天24小时营业，需要聘请一定数量的收银员来满足其需求。超市经理想聘请你帮助他解决一个问题。这个问题是，超市在每天的不同时间段需要不同数量的收银员（例如，午夜后需要少量收银员，而在下午则需要很多）以向顾客提供良好的服务，他希望尽可能少聘请的收银员。
经理为你提供了每天每个一小时时段所需的最少收银员的数量。这些数据以 R(0) , R(1), ..., R(23)的形式给出：R(0)代表从午夜到凌晨1:00所需的最少收银员数量，R(1)表示从凌晨1:00到凌晨2:00所需的最少收银员数量，依此类推。请注意，这些数字每天都是一样的。有N名符合这项工作的申请人。每个申请人 **i** 每天工作一次，每次工作8小时，从指定的时间 **ti（0 <= ti <= 23）** 开始，即从提到的整点开始。也就是说，如果第 **i** 名申请人被聘用，他/她将从 **ti** 点整开始工作 **8** 小时。且 **收银员之间不互相替换，严格按照预定时间工作，并且超市为被聘用的人提供了足够的收银台和柜台。**

你需要编写一个程序来读取 **R(i)（i=0..23）和ti（i=1..N），** 这些都是 **非负整数** ，并计算出为满足上述约束条件所需聘用的 **最少** 收银员数量。请注意，**对于某个特定时段，实际聘用的收银员数量可能会多于该时段所需的最少收银员数量。**
## 输入格式
输入的第一行表示这个问题的测试用例数量（最多20个）。每个测试用例都以一行中的24个整数开始，这些整数分别代表R(0), R(1), ..., R(23)，即超市在每天每个一小时时段所需的最少收银员数量（R(i)的最大值为1000）。紧接着是另一行，包含一个整数N，表示申请这份工作的人数（0 <= N <= 1000）。之后是N行，每行包含一个ti（0 <= ti <= 23），表示第i名申请人开始工作的时间（以午夜为起点的小时数，精确到整点）。不同测试用例之间没有空行分隔。

对于每个测试用例，输出应该是一行，包含满足超市在每个时段对收银员需求所需的最少收银员数量。如果某个测试用例没有解决方案（即，即使使用所有申请人也无法满足超市在所有时段的收银员需求），则应该为该测试用例输出"No Solution"。
## 输出格式
对于每个测试用例，输出应该是一行，包含满足超市在每个时段对收银员需求所需的最少收银员数量。如果某个测试用例没有解决方案（即，无论如何安排收银员的工作时间，都无法满足超市在所有时段的收银员需求），则应该为该测试用例输出"No Solution"。

```input1
1 
1 0 1 0 0 0 1 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 1 
5
0
23
22
1
10
```

```output1
1
```

