## ��Ŀ����
BaoBao is taking an online exam of the Kawa programming language, which consists of $n$ multiple choice questions. The exam is not easy, as for each question, BaoBao needs to select the one and only one correct answer from $10^5$ available choices! But don't worry, as an active committer of the famous \textit{open-kdk}, BaoBao obviously knows all the correct answers.

Although BaoBao is an expert in Kawa, the developers of the exam system are definitely not experts in software engineering. There are $m$ bugs in the exam system, and the $i$-th bug can be described as $(u_i, v_i)$, which means that BaoBao must select the same choice for question $u_i$ and $v_i$ (even if the choice he selects is incorrect!).

Time is limited, and the exam must go on. The developers only have time to fix one bug. Now the developers are wondering, for all $1 \le i \le m$, what's the maximum possible number of questions BaoBao can correctly answer if they fix the $i$-th bug. Please write a program to solve this problem so that the developers can select a proper bug to fix.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$, indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($1 \le n \le 10^5$, $1 \le m \le 10^5$), indicating the number of questions and the number of bugs.

The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^5$), where $a_i$ indicates the correct answer for question $i$.

For the following $m$ lines, the $i$-th line has two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$), indicating the $i$-th bug.

It's guaranteed that neither the sum of $n$ nor the sum of $m$ over all test cases will exceed $10^6$.

## �����ʽ
For each test case output one line containing $m$ integers $c_1, c_2, \dots, c_m$ separated by a space, where $c_i$ indicates the maximum possible number of questions BaoBao can correctly answer if the $i$-th bug is fixed.

Please, DO NOT output extra spaces at the end of each line, or your answer may be considered incorrect!

## ��Ŀ����
BaoBao ���ڲμ� Kawa ������Ե����߿��ԣ��ÿ����� $n$ ������ѡ������ɡ����Բ������ף�����ÿһ���⣬BaoBao ����Ҫ�� $10^5$ ������ѡ����ѡ��Ψһһ����ȷ�𰸣������ģ���Ϊ������ $\text{open-kdk}$ �Ļ��������ߣ�BaoBao ��Ȼ֪��������ȷ�Ĵ𰸡�

��Ȼ BaoBao �� Kawa �����ר�ң�������ϵͳ�Ŀ�����Ա���Բ���������̷����ר�ҡ�����ϵͳ���� $m$ �����󣬵� $i$ �������������Ϊ $(u_i,v_i)$������ζ�� BaoBao ����Ϊ�� $u_i$ �� $v_i$ ������ѡ����ͬ��ѡ���ʹ��ѡ���ѡ���ȷ������

���ǿ��Ա�������������ζ�ſ�����Աֻ��ʱ���޸�һ���������ڣ�������Ա��֪�����������е� $1\le i\le m$����������޸� $i$��BaoBao ������ȷ�ش��������������Ƕ��١�

## �����ʽ

�ж����������������ĵ�һ�а���һ������ $T$����ʾ��������������������ÿ������������

��һ�а����������� $n$ �� $m$��$1\le n\le 10^5$��$1\le m\le 10^5$������ʾ���������ʹ���������

�ڶ��а��� $n$ ������ $a_1,a_2,\dots,a_n$��$1\le a_i\le 10^5$�������� $a_i$ ��ʾ���� $i$ ����ȷ�𰸡�

�������� $m$ �У��� $i$ ������������ $u_i$ �� $v_i$��$1\le u_i,v_i\le n$������ʾ�� $i$ ������

��֤���в��������� $n$ �� $m$ ���ܺͶ����ᳬ�� $10^6$��

## �����ʽ

����ÿ�����������������һ�а����ɿո�ָ��� $m$ ������ $c_1,c_2,\dots,c_m$������ $c_i$ ��ʾ����޸��˵� $i$ ������BaoBao ������ȷ�ش�������������

�벻Ҫ��ÿ��ĩβ�������Ŀո񣬷������Ĵ𰸿��ܻᱻ��Ϊ�Ǵ���ģ�

## ��ʾ

�±�����˵�һ��ʾ������������

- �����ܵ�ѡ���б�ʾ BaoBao ����ѡ���ÿ�������һ����ܵ�ѡ�񣬴Ӷ�������ȷ�ش�������������������

- ����ȷ���б�ʾʹ�á����ܵ�ѡ�������ṩ��һ��ѡ����ȷ�ش�������������

$$\begin{array}{|c|c|c|c|}
\hline
\textbf{Bug ���} & \textbf{���ܵ�ѡ��} & \textbf{��ȷ} \\
\hline
1 & (1, 2, 1, 2, 1, 1, 1) & 6 \\
\hline
2 & (2, 2, 1, 2, 1, 1, 1) & 5 \\
\hline
3 & (1, 1, 1, 2, 1, 1, 1) & 5 \\
\hline
4 & (1, 1, 1, 1, 1, 2, 1) & 5 \\
\hline
5 & (1, 1, 1, 1, 1, 1, 1) & 4 \\
\hline
\end{array}$$

���ڵڶ����������������������ĸ� bug ���޸���BaoBao ������Ϊ������������ѡ����ͬ��ѡ�����ÿ���������ȷ�𰸲�ͬ��BaoBao ֻ����ȷ�ش�һ�����⡣

���ڵ�����ʾ��������������ע�⣬��ʹ������Ա�޸��˵�һ�����󣬵ڶ���������Ȼ��Ч��BaoBao ��Ȼ����Ϊ����������ѡ����ͬ��ѡ�����ڶ��������޸������Ҳ��һ���ġ�

```input1
3
7 5
1 2 1 2 1 2 1
1 2
1 3
2 4
5 6
5 7
3 3
1 2 3
1 2
1 3
2 3
2 3
12345 54321
1 2
1 2
1 1
```

```output1
6 5 5 5 4
1 1 1
1 1 1
```

## ��ʾ
The following table explains the first sample test case.

- The ``possible choices`` column indicates a possible set of choices to each question BaoBao can select, leading to a maximum possible number of correctly answered questions;
- The ``correct`` column indicates the number of correctly answered questions using the set of choices provided in the ``possible choices`` column.

$$\begin{array}{|c|c|c|c|}
\hline
\textbf{Bug No.} & \textbf{Possible Choices} & \textbf{Correct} \\
\hline
1 & (1, 2, 1, 2, 1, 1, 1) & 6 \\
\hline
2 & (2, 2, 1, 2, 1, 1, 1) & 5 \\
\hline
3 & (1, 1, 1, 2, 1, 1, 1) & 5 \\
\hline
4 & (1, 1, 1, 1, 1, 2, 1) & 5 \\
\hline
5 & (1, 1, 1, 1, 1, 1, 1) & 4 \\
\hline
\end{array}$$

For the second sample test case, no matter which bug is fixed, BaoBao has to select the same choice for all the three questions. As the correct answer for each question is different, BaoBao can only correctly answer 1 question.

For the third sample test case, note that even if the developers fix the first bug, the second bug is still taking effect and BaoBao still has to select the same choice for the two problems. It's the same if the second bug is fixed.

