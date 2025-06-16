## ��Ŀ����
Why did the cow cross the road? Well, one reason is that Farmer John's farm simply has a lot of roads, making it impossible for his cows to travel around without crossing many of them.

FJ's farm is arranged as an $N \times N$ square grid of fields ($2 \leq N \leq 100$), Certain pairs of adjacent fields (e.g., north-south or east-west) are separated by roads, and a tall fence runs around the external perimeter of the entire grid, preventing cows from leaving the farm. Cows can move freely from any field to any other adjacent field (north, east, south, or west), although they prefer not to cross roads unless absolutely necessary.

There are $K$ cows ($1 \leq K \leq 100, K \leq N^2$) on FJ's farm, each located in a different field. A pair of cows is said to be "distant" if, in order for one cow to visit the other, it is necessary to cross at least one road. Please help FJ count the number of distant pairs of cows.

## �����ʽ
The first line of input contains $N$, $K$, and $R$. The next $R$ lines describe $R$ roads that exist between pairs of adjacent fields. Each line is of the form $r$ $c$ $r'$ $c'$ (integers in the range $1 \ldots N$), indicating a road between the field in (row $r$, column $c$) and the adjacent field in (row $r'$, column $c'$). The final $K$ lines indicate the locations of the $K$ cows, each specified in terms of a row and column.

## �����ʽ
Print the number of pairs of cows that are distant.

## ��Ŀ����
### ��Ŀ����

��ţΪʲôҪ����·������һ��ԭ���� Farmer John ��ũ���кܶ��·��ʹ��������ţ���Ĵ��߶�ʱ���ɱ����Ҫ��������·��

FJ ��ũ�������ų�һ�� $N \times N$ �ķ���������أ�$2 \leq N \leq 100$����ĳЩ���ڵ���أ������ϱ�������򣩱���·�ָ�������������ⲿ��һȦ�߸ߵ�Χ������ֹ��ţ�뿪ũ������ţ���Դ��κ���������ƶ������ڵ���أ����������ϻ��������������ǳ��Ǿ��Ա�Ҫ������Ը�⴩����·��

ũ������ $K$ ͷ��ţ��$1 \leq K \leq 100, K \leq N^2$����ÿͷ��ţλ�ڲ�ͬ����ء����һͷ��ţҪ�ݷ���һͷ��ţʱ�������ٴ���һ����·����ô�����ţ����Ϊ��Զ���롱�ԡ������ FJ ����Զ������ţ�Ե�������

### �����ʽ

����ĵ�һ�а��� $N$��$K$ �� $R$���������� $R$ �������� $R$ ���������������֮��ĵ�·��ÿ�еĸ�ʽΪ $r$ $c$ $r'$ $c'$����ΧΪ $1 \ldots N$ ������������ʾλ�ڣ��� $r$���� $c$������������ڵģ��� $r'$���� $c'$�������֮����һ����·������ $K$ �б�ʾ $K$ ͷ��ţ��λ�ã�ÿ�����к���ָ����

### �����ʽ

���Զ������ţ�Ե�������

```input1
3 3 3
2 2 2 3
3 3 3 2
3 3 2 3
3 3
2 2
2 3
```

```output1
2
```

