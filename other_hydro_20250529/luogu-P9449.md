## ��Ŀ����
The Internet can be so fickle. You work for a small ad agency, Mimi's Mammoth Memes. Your ad campaigns are very cheap, and rely on the hope of producing the next hit viral meme. Unfortunately, the last four hundred or so memes have failed to take off, despite having been precisely engineered to appeal to every single person on Earth. You're not sure what exactly went wrong, but you've decided to try a new approach: crowd sourcing!

According to your scientific meme theory, all memes can be rated from $-\infty$ to $\infty$ on two scales: xanthochromism, and yellowishness, also known as ($x$, $y$) values. Obviously (you think), the best memes are memorable for being particularly xanthochromic, yellowish, unxanthochromic, or unyellowish. You feel that the "quality" of any meme is directly measurable as its squared Euclidean distance ($x^2 + y^2$) from the Base Meme ($0$, $0$), otherwise known as All Your Base.

To produce the ultimate viral meme, you'll be taking your company's last few failed memes and throwing them into a tournament, decided by online voting. The tournament can be represented as a rooted tree. Input memes come in at the leaves, and at each internal node, a vote will be held among its $k$ child memes ($x_1$, $y_1$), $\ldots$, ($x_k$, $y_k$). After the vote, all the memes will be horrifically mangled and merged into a brand new meme, specifically calculated to emphasize the winner and de-emphasize all the losers: the resultant $x$ value will be $$ \sum_{i=1}^{k} w_i \cdot x_i, $$ where $w_i$ is $1$ if the $i^{th}$ child won, and $-1$ otherwise. The $y$ value is computed similarly. This new meme will move on to the next vote in the tournament $-$ or, if there is no parent, it will be declared the champion and the ultimate meme!

You already have the structure of the tournament planned out, including all the input memes and the internal voting nodes. What is the largest possible quality for any meme that the tournament could produce?

## �����ʽ
The first line of input contains an integer $n$ ($1 \leq n \leq 10^4$), giving the total number of nodes in the tournament tree. The next $n$ lines each describe a single tree node indexed from $1$ to $n$. The line for node $i$ starts with an integer $k_i$ ($0 \leq k_i \leq 100$), the number of children of that node. If $k_i$ is $0$, then node $i$ is an input meme and there will be two more integers $x_i$ and $y_i$ ($-10^3 \leq x_i, yi \leq 10^3$) describing it. If $k_i &gt; 0$, then $k_i$ different integers $j$ ($i &lt; j \leq n$) will follow, giving the indices of the $k_i$ nodes entering this voting step.

All input memes will eventually be merged into the final output meme at node $1$. The complete tree will have a height of no more than $10$.

## �����ʽ
Output the largest possible quality for the champion meme at node $1$.

## ��Ŀ����
������֪�����������ߺ������������׽�������ְ��һ����Ϊ Mimi's Mammoth Memes ��С�͹�湫˾�����ǵĹ����Էǳ�����ʵ�ݣ�ȫ����������ʹ����һ������Ĳ���ʽ��ͼ������Ȼ�����������Ǿ�����ƹ���������İٶ����ͼȴ��һ�𱬡��������ľ���ԭ�򲢲�ʮ�����������������һ��ȫ�µķ������ڰ����⣡

������Ĺ�ͼ��ѧ���ۣ����й�ͼ������������ά���ϱ����֣��ֱ������޶Ⱥͷ��Ƴ̶ȣ����Ϊ $(x, y)$ ֵ����Ȼ����������Ϊ��������ڵĹ�ͼҪô�ر����ޣ�Ҫô�ر����ޣ�Ҫô�ر𷺻ƣ�Ҫô�ر𲻷��ơ�����Ϊ��һ����ͼ�ġ�����������ֱ��ͨ�����ͻ�����ͼ $(0, 0)$ ��ŷ����þ���ƽ���������������� $(x^2 + y^2)$��

Ϊ�˴�����ռ�����ʽ��ͼ���㽫�ѹ�˾����������ɹ��Ĺ�ͼ����һ��ͨ������ͶƱ����ʤ���Ľ������С����������������һ���и�������ʾ�����빣ͼλ��Ҷ�ӽڵ㣬��ÿ���ڲ��ڵ㣬����� $k$ ���ӹ�ͼ $(x_1, y_1),\cdots, (x_k, y_k)$ ����ͶƱ��ͶƱ�󣬹�ͼ�������ֲ���Ť�����ϲ���һ���¹�ͼ���ر�ͻ����ʤ�߲����������еİ��ߣ��õ��� $x$ ֵΪ 

$$ \sum_{i=1}^{k} w_i \cdot x_i, $$ 

���е��� $i$ ����ͼ��ʤʱ��$w_i$ Ϊ $1$������Ϊ $-1$��$y$ ֵ�ļ��㷽ʽ��ͬ�����¹�ͼ�������������һ�ֵ�ͶƱ���������û�и��ڵ㣬��ᱻ����Ϊ�ھ���Ҳ�������յ�������ͼ��

���Ѿ���ƺ��˽������Ľṹ��������������Ĺ�ͼ���ڲ���ͶƱ�ڵ㡣��ô���ý��������ܲ����Ĺ�ͼ���������ֵ�Ƕ��٣�

## �����ʽ

����ĵ�һ�а���һ������ $n$ ($1 \leq n \leq 10^4$)����ʾ���������еĽڵ��������������� $n$ �У�ÿ������һ����Ŵ� $1$ �� $n$ �Ľڵ㡣���ڽڵ� $i$����һ���ȳ���һ������ $k_i$ ($0 \leq k_i \leq 100$)����ʾ�ýڵ���ӽڵ�������� $k_i$ Ϊ 0��������ڵ� $i$ ��һ�����빣ͼ�������������������� $x_i$ �� $y_i$ ($-10^3 \leq x_i, y_i \leq 10^3$)�������ù�ͼ������ֵ����� $k_i > 0$�������������� $k_i$ ����ͬ������ $j$ ($i < j \leq n$)����ʾ������һͶƱ����Ľڵ�������

��������Ĺ�ͼ�����ձ��ϲ�Ϊ�ڵ� $1$ �е����������ͼ���������ĸ߶Ȳ��ᳬ�� $10$��

## �����ʽ

����ڵ� $1$ �Ĺھ���ͼ��������������


```input1
4
3 2 3 4
0 10 1
0 3 6
0 2 7

```

```output1
169
```

```input2
8
3 4 2 5
2 3 8
0 -3 9
0 -5 -7
2 6 7
0 1 4
0 -3 -1
0 1 4

```

```output2
314
```

