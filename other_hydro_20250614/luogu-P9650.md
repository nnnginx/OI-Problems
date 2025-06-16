## ��Ŀ����
BaoBao, one of the most famous monster hunters, wakes up in the middle of Heltion City dominated by monsters. Having troubles remembering what has happened, BaoBao decides to escape from this horrible city as soon as possible. Despite arming no weapon, he luckily puts his hand on a map in his right pocket, which contains valuable information that can possibly help him find a way out.  

According to the map, Heltion City is composed of $n$ spots connected by $m$ undirected paths. Starting from spot $1$, BaoBao must head towards any of the $k$ exits of the city to escape, where the $i$-th of them is located at spot $e_i$.

However, it's not an easy task for BaoBao to escape since monsters are everywhere in the city! For all $1 \le i \le n$, $d_i$ monsters are wandering near the $i$-th spot, so right after BaoBao arrives at that spot, at most $d_i$ paths connecting the spot will be blocked by monsters and are unable for BaoBao to pass. When BaoBao leaves the $i$-th spot, the monsters will go back to their nests and the blocked paths are clear. Of course, if BaoBao comes back to the spot, at most $d_i$ paths will be again blocked by the monsters. The paths blocked each time may differ.

As BaoBao doesn't know which paths will be blocked, please help him calculate the shortest time he can escape from the city in the worst case.


## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ (about $100$), indicating the number of test cases. For each test case:

The first line contains three integers $n$, $m$ and $k$ ($1 \le n \le 10^5$, $1 \le m \le 10^6$, $1 \le k \le n$), indicating the number of spots, the number of undirected paths and the number of exits of the city.

The second line contains $k$ distinct integers $e_1, e_2, \dots, e_k$ ($1 \le e_i \le n$), indicating $k$ exits of Heltion City.

The third line contains $n$ integers $d_1, d_2, \dots, d_n$ ($0 \le d_i \le m$), where $d_i$ indicates the number of monsters at the $i$-th spot.

For the following $m$ lines, the $i$-th line contains three integers $x_i$, $y_i$ and $w_i$ ($1 \le x_i,y_i \le n$, $x_i \neq y_i$, $1 \le w_i \le 10^4$), indicating an undirected edge of length $w_i$ connecting spot $x_i$ and $y_i$.

It's guaranteed that the total sum of $n$ will not exceed $10^6$ and the total sum of $m$ will not exceed $3 \times 10^6$. 


## �����ʽ
For each case output one line containing one integer. If BaoBao can get to some exit in the worst case, output the shortest possible time cost; Otherwise if BaoBao cannot get to any exit in the worst case, output ``-1``  instead.


## ��Ŀ����
### ��Ŀ����

������������ Heltion ���С�

���п��Կ����� $n$ ������ $m$ ������ɵ�**��Ȩ����ͼ**���ʼ������ $1$ �Žڵ㡣�����д��� $k$ �����ڣ��� $i$ ������λ���� $e_i$ �ŵ� ����������Ҫ�������ٶȵ���**��Щ�����е�����һ��**������ Heltion �ǡ�

���ɵ��ǣ��������й����ε������ڵ� $i$���� $d_i$ ֻ����פ���ڴˡ������������ $i$ ʱ�������**�����������** $d_i$ **��**��֮���ڵĵ�·����������ͨ����Щ�������ĵ�·����������**�뿪��**���� $i$ �Ĺ������ѣ���ʱ��������**��·��⿪**��

���ﱦ������������£����ӳ� Heltion ����Ҫ��á�

### �����ʽ

��һ��Ϊһ�������� $T$����ʾ�� $T$ ��������ݡ�

����ÿ�����ݣ���һ�а������������� $n$��$m$��$k$���ֱ��ʾ���еĵ����������ͳ����г��ڵ�������

�ڶ����� $k$ �������� $e_1, e_2,\dots , e_k$����ʾ�� $i$ �������� $e_i$ �Žڵ㡣

�������� $n$ �������� $d_1, d_2,\dots , d_n$����ʾ�� $i$ ���ڵ����� $d_i$ ֻ���

�������� $m$ �У�һ������������ $x_i$��$y_i$��$w_i$����ʾ�� $i$ ��˫��������ӵ��������Ȩ��

### �����ʽ

�� $T$ �У�ÿ��һ���������� $i$ �е�������ʾ�� $i$ �����ݵĴ𰸡�

����ÿ�����ݣ����������ܵ����κ�һ�����ڣ������ `-1`���������������������һ����������Ҫ������ʱ�䡣

### ���ݷ�Χ

���� $100\%$ �����ݣ�$1\le n \le 10^5$��$\sum n \le 10^6$��$1\le m \le 10^6$��$\sum m \le 3\times 10^6$��$1\le k \le n$��$1\le e_i \le n$��$0\le d_i \le m$��$1\le x_i,y_i \le n$��$1\le w_i \le 10^4$�����ݱ�֤ $x_i \neq y_i$��

```input1
2
3 4 1
3
1 1 1
1 2 1
1 2 2
2 3 1
2 3 2
3 2 2
2 3
2 0 0
1 2 1
1 3 1

```

```output1
4
-1

```

