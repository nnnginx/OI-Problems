## ��Ŀ����
Farmer John's N (2 <= N <= 10,000) cows, conveniently numbered 1..N, are fluent in some M (1 <= M <= 30,000) languages, also conveniently numbered from 1..M. Cow i can speak in K\_i (1 <= K\_i <= M) languages, namely L\_i1, L\_i2,..., L\_{iK\_i} (1 <= L\_ij <= M). FJ's cows aren't THAT smart, so the sum of K\_i over all cows i is at most 100,000.

Two cows can't directly talk to each other unless both speak a common language. However, cows can pass messages along, translating if necessary. In other words, cows A and B can have a conversation if and only if there exists a sequence of cows T\_1, T\_2, ..., T\_k such that A and T\_1 share a language, T\_1 and T\_2 share a language, etc., and T\_k and B share a language.

Farmer John wishes that his cows could be even more social, so he wants all his cows to be able to socialize with any other cow. He can buy books to teach any one of his cows any language he pleases. Being a fairly frugal farmer, FJ wants to purchase the minimum number of books necessary to enable all of his cows to speak to each other. Help him determine:

\* The minimum number of books he must purchase

\* Any set of books assigned to cows in any order which will help him meet this goal; a program will grade your output.

By way of example, suppose there are three cows named Alberta, Bessie, and Contessa along with three languages denoted as #1, #2, and #3. Alberta can speak languages #2 and #3, Bessie can speak language #2, and Contessa can speak language #1. Currently, Alberta and Bessie can talk to each other, but Contessa is left alone.

```
#1   #2   #3
Alberta           x    x
Bessie            x
Contessa     x
```
FJ wants to fix this situation, so he can buy Contessa a book to teach her language #2. This will ensure all cows speak the same language, so they can all communicate with one another.

Note that an alternate solution exists: instead, FJ could buy

Contessa a book to teach her language #3. Not all cows would speak the same language, but this would still be a valid solution because Contessa could communicate through Alberta (who also speaks language #3) if she wants to talk to Bessie. Other alternatives exist, and any valid alternate solution will also be accepted.

ũ��Լ����$N(2<=N<=10,000)$ֻ��ţ���Ϊ$1..N$��ͬ������$M(1<=M<=30,000)$��ţ����Ϊ$1..M$����iֻ��ţ��˵$K_i(1<=K_i<=M)$��ţ��ֱ�Ϊ$L_i1,L_i2,��,L_{iK_i}(1<=L_ij<=M)$��ũ�����ţ�����ر����������$K_i$���ۼӺͲ�����$100,000$��

��ֻ��ţֻ�е�����������һ������һ����ʱ��ſ��Թ�ͨ����������ֻ��ţ����Ҫ�����������Ƿ�����ܽ��������仰˵��A��BҪ���й�ͨ�����ǿ���ͨ��$T_1,T_2,��,T_k$�����ݣ�����A��$T_1,T_1$��$T_2,��,T_k$��B���н�����

ũ��ϣ��������ţ���Զ�๵ͨ�����������˺ܶ�α�ȥ��������ţ���ԡ���Ȼũ��ǳ������ģ���ϣ�������ٵ���Ϳ��������е���ţ���Խ��������������ǰ������������Ҫ�򼸱��顣


## �����ʽ
\* Line 1: Two space-separated integers: N and M

\* Lines 2..N+1: Line i+1 describes the languages that cow i can speak with $(K_i)+1$ space-separated integers: $K_i$, $L_i1$,

L\_i2,...,L\_i{K\_i}. 



## �����ʽ
\* Line 1: A single integer that is the minimum number of books that FJ must purchase.

\* Lines 2..B+1: Line i+1 contains two space-separated integers: the language id # and the id # of the cow to receive book i. If multiple solutions exist, print any one.


```input1
3 3 
2 3 2 
1 2 
1 1 

```

```output1
1 

```

