## ��Ŀ����
Farmer John has to take his annual farming license test. The test comprises N (1 <= N <= 1,000,000) true/false questions. After FJ's dismal performance on last year's test Bessie wishes to help him.

Bessie has inside information that the number of questions whose answer is true will be one of t\_1, t\_2, t\_3,..., or t\_K (0 <= t\_i <= N; 0 <= K <= 10,000) -- even though Bessie has no information about any answer to any specific question. Bessie wants to know the best score that FJ is guaranteed achieve by exploiting this information carefully, even if he doesn't know the actual answers to any test questions.

To demonstrate Bessie's idea, consider a license test with N=6 questions where Bessie knows that the number of questions with the answer 'true' is either 0 or 3. FJ can always get at least 3 answers correct using logic like this: If FJ answers 'false' on every

question and there are 0 questions with the answer 'true' then he will get all 6 correct. If there are 3 questions with the answer 'true' then he will get 3 answers correct. So as long as he marks every answer as 'false' he is guaranteed to get at least 3 correct without knowing any answer to the test questions.

On the other hand, consider what happens if FJ chooses an inferior strategy: he guesses that some 3 answers are 'true' and the other 3 are 'false'. If it turns out that NO answers are 'true' then FJ will get 3 answers correct, the ones he guessed were false. If 3 answers are 'true' then FJ could get as few as 0 answers correct. If he answered incorrectly on all 3 of that answers for which he guessed 'true', and the other 3 (for which he guessed 'false') are true, then he gets 0 correct answers. Even though FJ could get 3 correct in this case by guessing 'false' every time, he can not always guarantee even 1 correct by guessing some 3 answers as 'true', so this strategy can not guarantee getting any answer correct. FJ should use the previous paragraph's strategy.

Given Bessie's inside information, determine the number of answers FJ can always get correct using this information assuming he uses it optimally.


Farmer JohnҪ�μ�һ��һ�ȵ�ũ���ʸ��ԡ����Ժܼ򵥣�ֻ��N�� ��1��N��1��000��000)true/false���ж��⡣Ȼ��FJȥ�꿼��ȴ�����ߡ��ˣ�Bessie��ϣ�������ܰ������


Bessie�õ��ɿ����ڲ���Ϣ���п�����T\_1��T\_2��T\_3��...����T\_K(0��T\_i��N��0��K��10��000)


����Ĵ�Ϊture�����������ĵ���Ĵ���ʲôȴ��֪����Bessieϣ��֪���������о�����Щ�ڲ���Ϣ��(��Ȼ����ȷ���κ�һ����ľ����)��һ����֤FJ����ʱ�ܻ�õ���߷����Ƕ���?


Ϊ��˵��Bessie���뷨������N=6��һ�ο��ԣ�Bessie֪����Ϊtrue�����������0����3��FJ���԰�����������������������3�⣺���FJȫ����'false'����ô����0�������ȷ����'true'����FJ���6�⣻������3�������ȷ����'true'����FJ���3�⡣��ˣ�ֻҪFJ����'false'����ô����һ���ܴ��3�⣬����FJ����֪��ÿ�����ȷ�д𰸡�


��һ���棬�������FJѡ������һ�ַ����ŵ�������ԣ����²�ĳ3����Ϊ'true'����3����Ϊ'false'����������Ŀ����ȷ����'false'ʱ����ôFJ�ܴ��3���⡣������3�������ȷ����'true'ʱ����ôFJ�п���һ���ⶼ�𲻶ԡ�������ΪFJ�п��ܰ�3����ȷ��Ϊ'true'����ȫ�³�'false'!��˵������������Բ���ǰһ�����㡣

����Bessie��õ��ڲ���Ϣ�������FJ��������������Ա�֤�ܵõ�����߷����Ƕ���?

��1�У�2������N��K

��2��K+1�У���i+1�а���һ������t_i

��1�У�һ����������ʾFJһ���ܻ�õ���߷���

## �����ʽ
\* Line 1: Two space-separated integers: N and K

\* Lines 2..K+1: Line i+1 contains a single integer: t\_i

��1�У�2������N��K


��2��K+1�У���i+1�а���һ������t\_i


��1�У�һ����������ʾFJһ���ܻ�õ���߷���


## �����ʽ
\* Line 1: A single integer, the best score FJ is guaranteed to achieve


```input1
6 2 
0 
3 

```

```output1
3 

```

## ��ʾ
�����ṩ�� @fan404


