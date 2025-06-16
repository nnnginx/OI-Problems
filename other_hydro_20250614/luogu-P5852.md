## ��Ŀ����
Snow has arrived on the farm, and as she does at the beginning of every winter,
Bessie is building a snow-cow! Most of the time, Bessie strives to make her
sculpture look as much like a real cow as possible.  However, feeling
artistically inspired, this year she decides to pursue a more abstract route and
build a sculpture in the shape of a tree, consisting of $N$ snowballs
$(1\le N\le 10^5)$ connected by  $N-1$ branches, each connecting a pair of
snowballs such that there is a  unique path between every pair of snowballs. 

Bessie has added a nose to one of the snowballs, so it represents the head of
the abstract snow cow.  She designates it as snowball number 1.  To add more
visual interest, she plans to dye some of the snowballs different colors in an
artistic fashion by filling old milk pails with colored dye and splashing them
onto the sculpture.  Colors are identified by integers in the range
$1 \ldots 10^5$, and  Bessie has an unlimited supply of buckets filled with dyes
of every possible color.

When Bessie splashes a snowball with a bucket of dye, all the snowballs in its 
subtree are also splashed with the same dye (snowball $y$ is in the subtree of
snowball $x$ if $x$ lies on the path from $y$ to the head snowball). By
splashing each color with great care, Bessie makes sure that all colors a 
snowball has been splashed with will remain visible. For example, if a snowball
had colors $[1,2,3]$ and Bessie splashes it with color $4$, the snowball will
then have colors $[1,2,3,4]$. 

After splashing the snowballs some number of times, Bessie may also want to know
how colorful a part of her snow-cow is.  The "colorfulness" of a snowball $x$ is
equal to the number of distinct colors $c$ such that snowball $x$ is colored
$c$. If Bessie asks you about snowball $x$, you should reply with the sum of the
colorfulness values of all snowballs in the subtree of $x.$

Please help Bessie find the colorfulness of her snow-cow at certain points in
time.

## ��Ŀ����
ũ����ѩ����Bessie �����꿪��һ���ڶ�ѩţ����֮ǰ�Ǹ�дʵ�ɣ������������ѩţ�ѵú͸���ţһ���������겻һ�����ܵ����Զ���������������Ӱ�죬������������������������ѳ�һ���������ӡ�������� $N$ ��ѩ��$N-1$ ����֦���ɣ�ÿ����֦��������ѩ�򣬲���ÿ����ѩ��֮��·��Ψһ��

Bessie Ҫ������ѩţ����ϸ�ڡ������������һ��ѩ����˸����ӣ�����ʾ�������ǳ����ţ��ͷ�����Ұ�������ѩ�� $1$��Ϊ����ѩţ���ÿ�������Ҫ��ĳЩѩ�����㲻ͬ����ɫ�����ǣ����þ�ţ��Ͱװ���������õ�ѩţ�ϡ���Щ���Ϸֱ𱻱��Ϊ $1,2,\dots 10^5$����ÿ����ɫ����������Ӧ��

�� Bessie ��һͰ�����õ�һ��ѩ����ʱ�����ѩ�������ϵ�����ѩ��Ҳ�ᱻȾɫ�����ǳ�ѩ�� $y$ ��ѩ�� $x$ �������ﵱ�ҽ���ѩ�� $x$ ����ѩ�� $y$ ��ѩ�� $1$ ��·���ϣ���Bessie ���ž�ȷ�������ϼ��������������һ�����Ϻ�һ��ѩ����֮ǰ��Ⱦ����������ɫ��Ȼ�����ɼ������磬һ��ѩ��֮ǰ���ֳ�����ɫ $\left[ 1,2,3 \right]$��Ȼ�� Bessie ��װ�� $4$ ����ɫ��ţ��Ͱ����ȥ����ô���ѩ�����ֳ�����ɫ $\left[ 1,2,3,4 \right]$�� �����˼�Ͱ�����Ժ�Bessie ������Ҫ�˽�����ѩţ�ж���ʰ�쵡���ѩ�� $x$ �ġ���ɫ�ḻ�ȡ�Ϊ���ѩ��Ⱦ�ϵĲ�ͬ��ɫ���� ���� Bessie ���˽�ѩ�� $x$ �������Ϣʱ����Ӧ�ûش���ѩ�� $x$ �����������е�ѩ�����ɫ�ḻ��֮�͡�

�ȾȺ��Ӱɣ�

## �����ʽ
��һ�У�$N$ ��ѯ���� $Q$��

������ $N-1$ ��ÿ�������ÿո�������� $a$ �� $b$����ʾѩ�� $a$ �� $b$ �м���һ����֦������

��� $Q$ ��ÿ��һ�����󣬸�ʽ����Ӧ�������£�

 - `1 x c`���޸ģ�����ʾ Bessie ��һͰװ����ɫ $c$ �������õ�ѩ�� $x$ ��ʹ��������������ѩ��Ⱦɫ��
 - `2 x`��ѯ�ʣ���ѯ��ѩ�� $x$ ����������ɫ�ḻ��֮�͡�

## �����ʽ
����ÿ��ѯ�ʣ������ѯ����������ɫ�ḻ��֮�͡�**Ϊ�˷�ֹ���������Ҫʹ�� 64 λ������**

```input1
5 18
1 2
1 3
3 4
3 5
1 4 1
2 1
2 2
2 3
2 4
2 5
1 5 1
2 1
2 2
2 3
2 4
2 5
1 1 1
2 1
2 2
2 3
2 4
2 5

```

```output1
1
0
1
1
0
2
0
2
1
1
5
1
3
1
1

```

## ��ʾ
#### ��������
ִ�����һ���޸ĺ�ѩ�� $4$ ��Ⱦ������ɫ $1$��

ִ����ڶ����޸ĺ�ѩ�� $4$ ��ѩ�� $5$ ��Ⱦ������ɫ $2$��

ִ����������޸ĺ�����ѩ�򶼱�Ⱦ������ɫ $1$��
#### ���ݷ�Χ
���ڲ��Ե� $2,3$��$1\le N\le 10^2,1\le Q\le 2\times 10^2$��

���ڲ��Ե� $4-6$��$1\le N\le 10^3,1\le Q\le 2\times 10^3$��

���� $100\%$ �����ݣ�$1\le N,\ Q,\ c \le 10^5, 1\le a,\ b,\ x \le N$��

USACO 2019 December ������T2

