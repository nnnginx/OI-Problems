## ��Ŀ����
In order to get from one of the $f\ (1 \le f \le 5\times 10^3)$ grazing fields (which are numbered $1\dots f$) to another field, Bessie and the rest of the herd are forced to cross near the Tree of Rotten Apples. The cows are now tired of often being forced to take a particular path and want to build some new paths so that they will always have a choice of at least two separate routes between any pair of fields. They currently have at least one route between each pair of fields and want to have at least two. Of course, they can only travel on Official Paths when they move from one field to another. Given a description of the current set of $r\ (f-1 \le r \le 10^4)$ paths that each connect exactly two different fields, determine the minimum number of new paths (each of which connects exactly two fields) that must be built so that there are at least two separate routes between any pair of fields. Routes are considered separate if they use none of the same paths, even if they visit the same intermediate field along the way. There might already be more than one paths between the same pair of fields, and you may also build a new path that connects the same fields as some other path.


Ϊ�˴� $f$ ���ݳ��е�һ���ߵ���һ�������������ͬ������ʱ���ò�·��һЩ��������Ŀ��µ�������ţ���Ѿ�����˱�����ĳһ��·�����������뽨һЩ��·��ʹÿһ�Բݳ�֮�䶼�������������໥�����·�����������Ǿ��ж�һЩѡ��ÿ�Բݳ�֮���Ѿ�������һ��·������������ $r$ ��˫��·��������ÿ��·������������ͬ�Ĳݳ�����������ٵ��½���·������, ·�������ɵ�·��β�������ɡ�����·���໥���룬��ָ����·��û��һ���غϵĵ�·�����ǣ����������·���Ͽ�����һЩ��ͬ�Ĳݳ��� ����ͬһ�Բݳ�֮�䣬�����Ѿ���������ͬ�ĵ�·����Ҳ����������֮���ٽ�һ����·����Ϊ��һ����ͬ�ĵ�·��
## �����ʽ
* Line $1$: Two space-separated integers: $f$ and $r$.
* Lines $2\dots r+1$: Each line contains two space-separated integers which are the fields at the endpoints of some path.
* �� $1$ ������ $f$ �� $r$�������� $r$ �У�ÿ������������������ʾ�����ݳ�������֮����һ����·��
## �����ʽ
* Line $1$: A single integer that is the number of new paths that must be built.
* ���ٵ���Ҫ�½��ĵ�·����
```input1
7 7
1 2
2 3
3 4
2 5
4 5
5 6
5 7
```
```output1
2
```
## ���ݹ�ģ
���� $100\%$ �����ݣ�$1\le f\le 5\times 10^3$��$f-1\le r\le 10^4$��
## ��Ŀ��Դ
Gold