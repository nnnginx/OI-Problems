## ��Ŀ����
Farmer John has fallen behind on organizing his inbox. The way his screen is organized, there is a vertical list of folders on the left side of the screen and a vertical list of emails on the right side of the screen. There are $M$ total folders, numbered $1 \ldots M$ $(1 \le M \le 10^4)$. His inbox currently contains $N$ emails numbered $1\ldots N$ $(1 \le N \le 10^5)$; the $i$th email needs to be filed into folder $f_i$ $(1\le f_i\le M)$. 

FJ's screen is rather small, so he can only view $K$ $(1\le K\le \min(N,M))$ folders and $K$ emails at once.  Initially, his screen starts out displaying folders
$1 \ldots K$ on the left and emails $1 \ldots K$ on the right. To access other folders and emails, he needs to scroll through these respective lists. For example, if he scrolls down one position in the list of folders, his screen will display folders $2 \ldots K+1$, and then scrolling down one position further it will display folders $3 \ldots K+2$.  When FJ drags an email into a folder, the email disappears from the email list, and the emails after the one that disappeared shift up by one position.  For example, if emails $1, 2, 3, 4, 5$ are currently displayed and FJ drags email 3 into its appropriate folder, the email list will now show emails $1, 2, 4, 5, 6$. FJ can only drag an email into the folder to which it needs to be filled.

Unfortunately, the scroll wheel on FJ's mouse is broken, and he can only scroll downwards, not upwards.  The only way he can achieve some semblance of upward scrolling is if he is viewing the last set of $K$ emails in his email list, and
he files one of these.  In this case, the email list will again show the last $K$ emails that haven't yet been filed, effectively scrolling the top email up by one. If there are fewer than $K$ emails remaining, then all of them will be
displayed. 

Please help FJ determine if it is possible to file all of his emails.

## �����ʽ
The first line of input contains $T$ $(1��T��10)$, the number of subcases in this input, all of which must be solved correctly to solve the input case. The $T$ subcases then follow. For each subcase, the first line of input contains $M,N$ and $K$. The next line contains $f_1\cdots f_N$.

It is guaranteed that the sum of $M$ over all subcases does not exceed $10^4$, and that the sum of $N$ over all subcases does not exceed $10^5$.

## �����ʽ
Output $T$ lines, each one either containing either YES or NO, specifying whether FJ can successfully file all his emails in each of the $T$ subcases.

## ��Ŀ����
### ��Ŀ����

Farmer John �����������ռ���ʱ����ˡ�������Ļ�������£���Ļ������ļ��еĴ�ֱ�б��Ҳ����ʼ��Ĵ�ֱ�б��ܹ��� $M$ ���ļ��У����Ϊ $1 \ldots M$��$1 \leq M \leq 10^4$���������ռ���Ŀǰ���� $N$ ���ʼ������Ϊ $1 \ldots N$��$1 \leq N \leq 10^5$������ $i$ ���ʼ���Ҫ�鵵���ļ��� $f_i$��$1 \leq f_i \leq M$����

FJ ����Ļ��С�������һ��ֻ�ܲ鿴 $K$ ���ļ��к� $K$ ���ʼ���$1 \leq K \leq \min(N, M)$������ʼʱ��������Ļ��ʾ�����ļ��� $1 \ldots K$ ���Ҳ���ʼ� $1 \ldots K$��Ϊ�˷��������ļ��к��ʼ�������Ҫ������Щ�б����磬��������ļ����б������¹���һ��λ�ã���Ļ����ʾ�ļ��� $2 \ldots K+1$�������¹���һ��λ������ʾ�ļ��� $3 \ldots K+2$���� FJ ��һ���ʼ������ļ���ʱ�����ʼ�����ʼ��б�����ʧ�������ʼ�����ǰ�ƶ�һ��λ�á����磬�����ǰ��ʾ���ʼ��� $1, 2, 3, 4, 5$���� FJ ���ʼ� $3$ �������Ӧ���ļ��У��ʼ��б���ʾ $1, 2, 4, 5, 6$��FJ ֻ�ܽ��ʼ���������Ҫ�鵵���ļ��С�

���ҵ��ǣ�FJ �������ֻ��ˣ���ֻ�����¹������������Ϲ�����Ψһ��ʵ���������Ϲ�����Ч���ǣ������鿴�ʼ��б����� $K$ ���ʼ�ʱ��������鵵������һ���ʼ����ʼ��б��ٴ���ʾ��δ�鵵����� $K$ ���ʼ����Ӷ�����������ʼ����Ϲ���һ��λ�á����ʣ����ʼ����� $K$ �⣬����ʾ����ʣ����ʼ���

����� FJ �ж��Ƿ��ܹ��鵵�����ʼ���

### �����ʽ

����ĵ�һ�а��� $T$��$1 \leq T \leq 10$������ʾ�����е�������������������������������ȷ������ܽ������������������������ $T$ ����ÿ�������������롣����ÿ������������һ�а��� $M$��$N$ �� $K$���ڶ��а��� $f_1 \cdots f_N$��

��֤������������ $M$ ֮�Ͳ����� $10^4$�������������� $N$ ֮�Ͳ����� $10^5$��

### �����ʽ

��� $T$ �У�ÿ�а��� `YES` �� `NO`����ʾ FJ �Ƿ��ܹ��ɹ��鵵�����ʼ���

### ���ݷ�Χ

- ������ 2-10 �У������������� $M$ ֮�Ͳ����� $10^3$��
- ������ 11-12 �У�û�ж������ơ�

```input1
6
5 5 1
1 2 3 4 5
5 5 1
1 2 3 5 4
5 5 1
1 2 4 5 3
5 5 2
1 2 4 5 3
3 10 2
1 3 2 1 3 2 1 3 2 1
3 10 1
1 3 2 1 3 2 1 3 2 1
```

```output1
YES
YES
NO
YES
YES
NO
```

## ��ʾ
�����ݷ�Χ��

- In inputs 2-10, the sum of $M$ over all subcases does not exceed $10^3$.
- In inputs 11-12, no additional constraints.

