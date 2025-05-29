## ��Ŀ����
Byteasar, the farmer, wants to plough his rectangular field. He can begin with ploughing a slice from any of the field's edges, then he can plough a slice from any unploughed field's edges, and so on, until the whole field is ploughed. After the ploughing of every successive slice, the yet-unploughed field has a rectangular shape. Each slice has a span of $1$, and the length and width of the field are the integers $n$ and $m$.

Unfortunately, Byteasar has only one puny and frail nag (horse) at his disposal for the ploughing. Once the nag starts to plough a slice, it won't stop until the slice is completely ploughed. However, if the slice is to much for the nag to bear, it will die of exhaustion, so Byteasar has to be careful. After every ploughed slice, the nag can rest and gather strength. The difficulty of certain parts of the field varies, but Byteasar is a good farmer and knows his field well, hence he knows every part's ploughing-difficulty.

Let us divide the field into $m\times n$ unitary squares - these are called tiles in short.

We identify them by their coordinates $(i,j)$, for $1\le i\le m$ and $1\le j\le n$.

Each tile has its ploughing-difficulty - a non-negative integer.

Let $t_{i,j}$ denote the difficulty of the tile which coordinates are $(i,j)$.


For every slice, the sum of ploughing-difficulties of the tiles forming it up cannot exceed a certain constant $k$ - lest the nag dies.

A difficult task awaits Byteasar: before ploughing each subsequent slice he has to decide which edge of the field he'll plough, so that the nag won't die. On the other hand, he'd like to plough as few slices as possible.

TaskWrite a programme that:

reads the numbers $k$,$m$ and $n$ from the input file, as well as the ploughing-difficulty coefficients,     determines the best way to plough Byteasar's field,     writes the result to the output file.

Byteasar��������ǿ���ε����ÿ���ܸ��־��ε�һ�ߣ��������Ҷ��У�������ÿ�θ����ʣ�µ���Ҳһ���Ǿ��Σ�ÿ��С����߳�Ϊ$1$�����صĳ���ֱ�Ϊ$m$��$n$�����ҵ���Byteasarֻ��һƥ������������ʼ���ؿ�ʼ��ֻ�е���������һ�߲Ż�ͣ����Ϣ������Щ�ػ�ǳ��Ѹ����������ǳ����ۣ����Byteasar��Ҫ�ر�С�ġ���������һ��֮�������ͣ������Ϣ�ָ�������ÿ��ظ��ֵ��ѶȲ�һ������Byteasar���ǳ���������ǽ��طֳ�$m\times n$�鵥λ���Ρ�������������$(i,j)$���������ǡ�ÿ��ض���һ������$t_{i,j}$,������$(i,j)$�ĸ����Ѷȡ�����ÿ�����һ�ߵ�ʱ���ѶȾ������������ֵĵص��Ѷ��ܺͣ�������ƥ����������ԣ����ֵ���ܳ�����������ֵ��Byteasar��֪�����������������������Ҫ�����ٴβ��ܰѵظ��ꡣ


## �����ʽ
There are three positive integers in the first line of the input file: $k$,$m$ and $n$,separated by single spaces, $1\le k\le 200\ 000\ 000$,$1\le m,n\le 2000$.

In the following $n$ lines there are the ploughing-difficulty coefficients.

The line no. $j+1$ contains the coefficients $t_{1,j},t_{2,j}...,t_{n,m}$, separated by single spaces,$0\le t_{i,j}\le 100\ 000$.


## �����ʽ
Your programme should write one integer to the output file: the minimum number of slices required to plough the field while satisfying the given conditions. Since we care for animals, we guarantee that the field can be ploughed according to the above rules. But remember, saving the nag is up to you!


```input1
12 6 4
6 0 4 8 0 5
0 4 5 4 6 0
0 5 6 5 6 0
5 4 0 0 5 4
```

```output1
8
```

## ��ʾ
��л@NaVi\_Awson �ṩ����


