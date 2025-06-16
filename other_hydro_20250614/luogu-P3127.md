## ��Ŀ����
Farmer John has received a shipment of N large hay bales ($1 \le N \le 100,000$), and placed them at various locations along the road leading to his barn. Unfortunately, he completely forgets that Bessie the cow is out grazing along the road, and she may now be trapped within the bales! Each bale $j$ has a size $S_j$ and a position $P_j$ giving its location along the one-dimensional road.  Bessie the cow can move around freely along the road, even up to the position at which a bale is located, but she cannot cross through this position.  As an exception, if she runs in the same direction for $D$ units of distance, she builds up enough speed to break through and permanently eliminate any hay bale of size strictly less than $D$.  Of course, after doing this, she might open up more space to allow her to make a run at other hay bales, eliminating them as well.

Bessie can escape to freedom if she can eventually break through either the  leftmost or rightmost hay bale.  Please compute the total area of the road consisting of real-valued starting positions from which Bessie cannot escape.



## �����ʽ
The first line of input contains $N$.  Each of the next $N$ lines describes a bale, and contains two integers giving its size and position, each in the range $1\ldots 10^9$. All positions are distinct.


## �����ʽ
Print a single integer, giving the area of the road from which Bessie cannot escape.

## ��Ŀ����
### ��Ŀ����

Farmer John �յ���һ�� $N$ �����͸ɲ�����$1 \le N \le 100,000$�����������Ƿ�������ͨ���Ȳֵĵ�·�ϵĲ�ͬλ�á����ҵ��ǣ�����ȫ��������ţ Bessie ��������·�ϳԲݣ������ڿ��ܱ�������Щ�ɲ���֮���ˣ�ÿ���ɲ��� $j$ ��һ����С $S_j$ ��һ��λ�� $P_j$����ʾ��������һά��·�ϵ�λ�á�Bessie �����ڵ�·�������ƶ������������ƶ����ɲ������ڵ�λ�ã������޷��������λ�á�Ψһ�������ǣ��������ͬһ���������ƶ� $D$ ��λ�ľ��룬��������㹻���ٶȣ��ܹ�ͻ�Ʋ����������κδ�С�ϸ�С�� $D$ �ĸɲ�������Ȼ����ͻ��֮�������ܻ�򿪸���Ŀռ䣬�Ӷ��л���ͻ�������ɲ������������������ǡ�

��� Bessie �����ܹ�ͻ�����������Ҳ�ĸɲ��������Ϳ��Գɹ����ѡ�������·�������޷����ѵ�ʵ����ʼλ�õ��������

### �����ʽ

����ĵ�һ�а��� $N$���������� $N$ ������ÿ���ɲ�����ÿ�а��������������ֱ��ʾ�ɲ����Ĵ�С��λ�ã���Χ��Ϊ $1 \ldots 10^9$������λ�þ�����ͬ��

### �����ʽ

���һ����������ʾ Bessie �޷����ѵĵ�·�������

```input1
5
8 1
1 4
8 8
7 15
4 20
```

```output1
14
```

