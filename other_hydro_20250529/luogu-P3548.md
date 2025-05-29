## ��Ŀ����
An exhibition of tapestries is opening in Byteotian Museum of Fine Arts.

The main exhibition room, viewed from top, is a polygon (not necessarily    convex).  A tapestry is hanged on each wall of the room, each tapestry    taking all the area of its wall.

A lamp has been installed in the room in order to illuminate the exhibition.

    The lamp is glowing uniformly in all directions.

However, while some of the tapestries have to be flooded with light,    others cannot be exposed to strong light.

Byteasar, the curator, has been moving the lamp around the room, but so far    he is not satisfied with the results.

Now he is terrified by the prospect of moving the tapestries around    instead - this would require much effort, and the exhibition is to open soon.

Perhaps you will be able to tell him if his attempts are doomed or not?

Your task is to determine if there is such a spot that placing the lamp    in it satisfies the following:

each wall is to be either completely illuminated or completely shaded, as required by the tapestry hanging on it;        there can be no wall that is partly illuminated and partly shaded;                  if the lamp is located exactly on the wall or its extension, this wall is not illuminated;                the lamp can neither be switched off nor taken away from the room; it has      to be on while located (strictly) inside the room (i.e., it cannot be      placed in a corner or on any wall).

һ����̺������չ����Byteotian��������Ʒ�����չ����


��չ�ҵĸ���ͼ��һ������Σ���һ����͹�ģ��������ÿ��ǽ���϶�����һ����̺��ÿ����̺��ռ��������ǽ��ȫ�������


һյ�Ʊ���װ�ڷ�����������չ��Ʒ���ƶ������з��򷢵Ĺⶼ�Ǿ��ȵġ�


Ȼ����Щ��̺��Ҫ����������������ȴ����ܿ�ǿ�⡣


��չ��Byteasar��һֱ�ڷ������ƶ��ƣ�����ĿǰΪֹ����һֱû�ó�����Ľ����


����չ���������ţ�����Լ�׽�������̣�����ˮ��û����֪���롣


�������������㣬������Ҫ�ҳ�������û������һ�����ʵĵط��ҵ�����������������


ÿ��ǽҪô��ȫ��������Ҫô����ȫ�ڱΣ���Ϊ��̺�Թ�����ʮ�����޵ģ����Բ�����ĳ��ǽ����������/�ڱΣ�����Ʊ�����ĳ��ǽ���ӳ����ϣ����ǽ���ᱻ�������ƼȲ��ܱ�Ϩ��Ҳ�����ƶ�λ�ã������ϸ�̶��ڷ���һ��ȷ����λ���ϣ��Ȳ��ܰ�����Ҳ���ܰ�ǽ�ϣ���


�����ʽ��


��һ����һ������t(1<=t<=20)��������t�����ݡ�


ÿ���������£�


��һ����һ������n(3<=n<=1000)����չ�����ǽ����


�����n��ָ���������״��


ÿ�а���һ������xi��yi(-30000<=xi,yi<=30000;i=1,2,...n)����֮�䱻һ���ո��������Ӧ���䣨����Σ���������꣬�������갴˳ʱ�����С�


�����n��ָ����ÿ��ǽ�Ϲ�̺�Ĺ�������


ÿ��Ϊһ����ĸS��C���ֱ�����̺��Ҫ���������ڱΡ�


��i���̺��1<=i<=n-1�������ڵ�i��ǽ�͵�i+1��ǽ��


���һ���̺�����ڵ�һ��ǽ�����һ��ǽ֮�䡣


���㹹�ɵĶ����û�н���㣬Ҳ����˵���������ı߹���һ������֮�⣬û��������������εı߹���һ�����㡣���Ҷ����û���κ������㹲�ߡ�


�����ʽ��


����ÿһ�����ݣ���ĳ���Ӧ�����һ������һ�����ʵĵ��еı�׼�����


����ƿ��Է�����������������Ҫ�����"TAK"���������yes������֮���"NIE"���������no��


��ʾ��


����40%�����ݵ㣬n<=20;


��������10%�����ݵ㣬���е�̺����Ҫ��������


## �����ʽ
There is a single integer ![](http://main.edu.pl/images/OI20/gob-en-tex.1.png) (![](http://main.edu.pl/images/OI20/gob-en-tex.2.png)) in the first line of      the standard input, denoting the number of data sets.

The following lines describe these data sets.

The first line of a single description holds a single integer ![](http://main.edu.pl/images/OI20/gob-en-tex.3.png) (![](http://main.edu.pl/images/OI20/gob-en-tex.4.png)), denoting the number of walls in the main exhibition room.

Then the following ![](http://main.edu.pl/images/OI20/gob-en-tex.5.png) lines specify the room's shape.

Each of those lines contains a pair of integers ![](http://main.edu.pl/images/OI20/gob-en-tex.6.png) and ![](http://main.edu.pl/images/OI20/gob-en-tex.7.png)      (![](http://main.edu.pl/images/OI20/gob-en-tex.8.png) for ![](http://main.edu.pl/images/OI20/gob-en-tex.9.png)), separated by      a single space, denoting the coordinates of the room's corner or, in      other words, the vertex of corresponding polygon.  The vertices are given      clockwise.

The next ![](http://main.edu.pl/images/OI20/gob-en-tex.10.png) lines specify the tapestries' requirements.

Each of those lines contains a single letter, S or      C, denoting that the wall has to be illuminated or shaded,      respectively.

The letter in the ![](http://main.edu.pl/images/OI20/gob-en-tex.11.png)-th of these lines (for ![](http://main.edu.pl/images/OI20/gob-en-tex.12.png))      regards the wall between the ![](http://main.edu.pl/images/OI20/gob-en-tex.13.png)-th and the ![](http://main.edu.pl/images/OI20/gob-en-tex.14.png)-th vertex.

The letter in the last of these lines regards the wall between the last      and the first vertex.

The polygon depicting the room's shape has no self-crossings, i.e.,      with the exception of successive sides, which share a common vertex,      no two sides of the polygon share a common point.  Furthermore, no three      vertices ��


## �����ʽ
For each data set your program should print to the standard output      a single line containing a single word:

TAK (Polish for yes) if the lamp can be placed so as   to satisfy all aforementioned requirements, or                      NIE (Polish for no) otherwise.


```input1
1
16
5 -3
4 -4
3 -7
0 -5
-3 -7
-4 -4
-5 -3
-1 -1
-4 3
-2 4
-1 2
0 7
1 2
2 4
4 3
1 -1
C
S
S
S
S
C
C
S
S
C
S
S
C
S
S
C
        


```

```output1
TAK

```

