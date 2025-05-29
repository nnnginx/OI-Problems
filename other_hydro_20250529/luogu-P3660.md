## ��Ŀ����
The layout of Farmer John's farm is quite peculiar, with a large circular road running around the perimeter of the main field on which his cows graze during the day. Every morning, the cows cross this road on their way towards the field, and every evening they all cross again as they leave the field and return to the barn.

As we know, cows are creatures of habit, and they each cross the road the same way every day. Each cow crosses into the field at a different point from where she crosses out of the field, and all of these crossing points are distinct from each-other. Farmer John owns $N$ cows, conveniently identified with the integer IDs $1 \ldots N$, so there are precisely $2N$ crossing points around the road. Farmer John records these crossing points concisely by scanning around the circle clockwise, writing down the ID of the cow for each crossing point, ultimately forming a sequence with $2N$ numbers in which each number appears exactly twice. He does not record which crossing points are entry points and which are exit points.

Looking at his map of crossing points, Farmer John is curious how many times various pairs of cows might cross paths during the day. He calls a pair of cows $(a,b)$ a "crossing" pair if cow $a$'s path from entry to exit must cross cow $b$'s path from entry to exit. Please help Farmer John count the total number of crossing pairs.

## �����ʽ
The first line of input contains $N$ ($1 \leq N \leq 50,000$), and the next $2N$ lines describe the cow IDs for the sequence of entry and exit points around the field.


## �����ʽ
Please print the total number of crossing pairs.


## ��Ŀ����
### ��Ŀ����

Farmer John ��ũ�����ַǳ����أ�����ص���Χ��һ�����ε�·��������ţ����������Բݡ�ÿ�����ϣ���ţ�Ƕ��ᴩ��������·������أ�ÿ�����������ֻ��ٴδ���������·�뿪��ط���ţ�

������֪����ţ��ϰ���Զ������ÿ�춼������ͬ�ķ�ʽ������·��ÿͷ��ţ������صĵ���뿪��صĵ㲻ͬ������������Щ�����㶼�˴˲�ͬ��Farmer John ӵ�� $N$ ͷ��ţ������������� ID $1 \ldots N$ ��ʶ����˵�·��Χǡ���� $2N$ �������㡣Farmer John ͨ��˳ʱ��ɨ�軷�ε�·����¼ÿ�����������ţ ID�������γ�һ������ $2N$ �����ֵ����У�����ÿ������ǡ�ó������Ρ�����δ��¼��Щ�������ǽ���㣬��Щ���뿪�㡣

�������Ĵ������ͼ��Farmer John ����һ���в�ͬ��ţ��֮����ܻύ����ٴΡ������ţ $a$ �ӽ���㵽�뿪���·����������ţ $b$ �ӽ���㵽�뿪���·�����棬��ô������ţ�� $(a,b)$ Ϊ�����桱�ԡ������ Farmer John ���㽻��Ե�������

### �����ʽ

����ĵ�һ�а��� $N$ ($1 \leq N \leq 50,000$)���������� $2N$ �������������Χ������뿪�����ţ ID ���С�

### �����ʽ

���������Ե�������

```input1
4
3
2
4
4
1
3
2
1
```

```output1
3
```

