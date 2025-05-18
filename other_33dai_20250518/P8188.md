## 题目描述
Farmer John has fallen behind on organizing his inbox. The way his screen is organized, there is a vertical list of folders on the left side of the screen and a vertical list of emails on the right side of the screen. There are $M$ total folders, numbered $1 \ldots M$ $(1 \le M \le 10^4)$. His inbox currently contains $N$ emails numbered $1\ldots N$ $(1 \le N \le 10^5)$; the $i$th email needs to be filed into folder $f_i$ $(1\le f_i\le M)$. 

FJ's screen is rather small, so he can only view $K$ $(1\le K\le \min(N,M))$ folders and $K$ emails at once.  Initially, his screen starts out displaying folders
$1 \ldots K$ on the left and emails $1 \ldots K$ on the right. To access other folders and emails, he needs to scroll through these respective lists. For example, if he scrolls down one position in the list of folders, his screen will display folders $2 \ldots K+1$, and then scrolling down one position further it will display folders $3 \ldots K+2$.  When FJ drags an email into a folder, the email disappears from the email list, and the emails after the one that disappeared shift up by one position.  For example, if emails $1, 2, 3, 4, 5$ are currently displayed and FJ drags email 3 into its appropriate folder, the email list will now show emails $1, 2, 4, 5, 6$. FJ can only drag an email into the folder to which it needs to be filled.

Unfortunately, the scroll wheel on FJ's mouse is broken, and he can only scroll downwards, not upwards.  The only way he can achieve some semblance of upward scrolling is if he is viewing the last set of $K$ emails in his email list, and
he files one of these.  In this case, the email list will again show the last $K$ emails that haven't yet been filed, effectively scrolling the top email up by one. If there are fewer than $K$ emails remaining, then all of them will be
displayed. 

Please help FJ determine if it is possible to file all of his emails.

## 输入格式
The first line of input contains $T$ $(1≤T≤10)$, the number of subcases in this input, all of which must be solved correctly to solve the input case. The $T$ subcases then follow. For each subcase, the first line of input contains $M,N$ and $K$. The next line contains $f_1\cdots f_N$.

It is guaranteed that the sum of $M$ over all subcases does not exceed $10^4$, and that the sum of $N$ over all subcases does not exceed $10^5$.

## 输出格式
Output $T$ lines, each one either containing either YES or NO, specifying whether FJ can successfully file all his emails in each of the $T$ subcases.

## 题目大意
### 题目描述

Farmer John 在整理他的收件箱时落后了。他的屏幕布局如下：屏幕左侧是文件夹的垂直列表，右侧是邮件的垂直列表。总共有 $M$ 个文件夹，编号为 $1 \ldots M$（$1 \leq M \leq 10^4$）。他的收件箱目前包含 $N$ 封邮件，编号为 $1 \ldots N$（$1 \leq N \leq 10^5$）；第 $i$ 封邮件需要归档到文件夹 $f_i$（$1 \leq f_i \leq M$）。

FJ 的屏幕很小，因此他一次只能查看 $K$ 个文件夹和 $K$ 封邮件（$1 \leq K \leq \min(N, M)$）。初始时，他的屏幕显示左侧的文件夹 $1 \ldots K$ 和右侧的邮件 $1 \ldots K$。为了访问其他文件夹和邮件，他需要滚动这些列表。例如，如果他在文件夹列表中向下滚动一个位置，屏幕将显示文件夹 $2 \ldots K+1$，再向下滚动一个位置则显示文件夹 $3 \ldots K+2$。当 FJ 将一封邮件拖入文件夹时，该邮件会从邮件列表中消失，其后的邮件会向前移动一个位置。例如，如果当前显示的邮件是 $1, 2, 3, 4, 5$，而 FJ 将邮件 $3$ 拖入其对应的文件夹，邮件列表将显示 $1, 2, 4, 5, 6$。FJ 只能将邮件拖入其需要归档的文件夹。

不幸的是，FJ 的鼠标滚轮坏了，他只能向下滚动，不能向上滚动。唯一能实现类似向上滚动的效果是，当他查看邮件列表的最后 $K$ 封邮件时，如果他归档了其中一封邮件，邮件列表将再次显示尚未归档的最后 $K$ 封邮件，从而将最上面的邮件向上滚动一个位置。如果剩余的邮件少于 $K$ 封，则显示所有剩余的邮件。

请帮助 FJ 判断是否能够归档所有邮件。

### 输入格式

输入的第一行包含 $T$（$1 \leq T \leq 10$），表示输入中的子用例数量，所有子用例都必须正确解决才能解决整个输入用例。接下来的 $T$ 行是每个子用例的输入。对于每个子用例，第一行包含 $M$、$N$ 和 $K$。第二行包含 $f_1 \cdots f_N$。

保证所有子用例的 $M$ 之和不超过 $10^4$，所有子用例的 $N$ 之和不超过 $10^5$。

### 输出格式

输出 $T$ 行，每行包含 `YES` 或 `NO`，表示 FJ 是否能够成功归档所有邮件。

### 数据范围

- 在输入 2-10 中，所有子用例的 $M$ 之和不超过 $10^3$。
- 在输入 11-12 中，没有额外限制。

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

## 提示
【数据范围】

- In inputs 2-10, the sum of $M$ over all subcases does not exceed $10^3$.
- In inputs 11-12, no additional constraints.

