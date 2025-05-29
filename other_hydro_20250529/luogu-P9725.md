## ��Ŀ����
Prof. Pang and Prof. Shou like playing a chase game.

The game map consists of $n$ rooms and $n-1$ bi-directional channels. The game map is connected. That means, the map forms a tree.

At first, Prof. Pang is in room $u$, while Prof. Shou is in room $v$ ($u\neq v$). Prof. Pang and Prof. Shou take turns to play, and Prof. Shou goes first. In one's turn, the player knows his own position and the other player's position and can decide either to stay in the current room or to move to another room which is connected with the current room directly by a channel. When Prof. Pang and Prof. Shou are in the same room, Prof. Shou is caught by Prof. Pang. 

Prof. Pang and Prof. Shou are smart enough. Prof. Pang wants to catch Prof. Shou in a finite number of turns. Prof. Shou does not want to be caught by Prof. Pang in any finite number of turns. 

Prof. Shou gets tired of being caught every time and finds Prof. Fei for help. Prof. Shou asks Prof. Fei to add some channels so that Prof. Pang cannot catch him in finite number of turns for any pair of initial rooms $(u,v)$. Prof. Fei is lazy, so he hopes to add as few channels as possible. If no matter how to add the channels there is always a pair of rooms $(u,v)$ such that Prof. Pang can catch Prof. Shou, output $-1$.

## �����ʽ
The first line contains a single integer $T$ ($1\le T\le 10^4$) denoting the number of test cases. 

For each test case, the first line contains a single integer $n$ ($2\le n\le 10^5$) denoting the number of rooms.

For the next $n-1$ lines, each line contains two integers $u$ and $v$ ($1\le u, v\le n$) denoting a channel connecting room $u$ and room $v$.

It is guaranteed that the sum of $n$ over all test cases does not exceed $2\times 10^5$, and the rooms and channels always form a tree.

## �����ʽ
For each test case, print a number denoting the smallest number of added channels, or just print $-1$.

## ��Ŀ����
**����Ŀ������**

�ӽ��ں��ٽ���ϲ����׷����Ϸ��

��Ϸ��ͼ�� $n$ ������� $n-1$ ��˫��ͨ����ɡ���Ϸ��ͼ����ͨ�ġ�����ζ�ŵ�ͼ�γ�һ������

һ��ʼ���ӽ����ڷ��� $u$�����ٽ����ڷ��� $v$��$u\neq v$�����ӽ��ں��ٽ�����������Ϸ���ٽ����ȿ�ʼ�����Լ��Ļغ��У����֪���Լ����ڵ�λ�ú���һ����ҵ�λ�ã����Ծ������ڵ�ǰ��������ƶ����뵱ǰ����ֱ��ͨ��ͨ����������һ�����䡣���ӽ��ں��ٽ�����ͬһ������ʱ���ٽ��ڱ��ӽ���ץס��

�ӽ��ں��ٽ����㹻�������ӽ���ϣ�������޵Ļغ���ץס�ٽ��ڡ��ٽ��ڲ�ϣ�����κ����޵Ļغ��ڱ��ӽ���ץס��

�ٽ��������ÿ�ζ���ץס���ҵ��˷ѽ���Ѱ��������ٽ�������ѽ������һЩͨ����ʹ�����۳�ʼ����� $(u,v)$ ��Σ��ӽ��ڶ��޷������޵Ļغ���ץס�����ѽ��ں�����������ϣ���������ٵ����ͨ�����������������ͨ�������Ǵ���һ�Է��� $(u,v)$��ʹ���ӽ����ܹ�ץס�ٽ��ڣ���� $-1$��

**�������ʽ��**

��һ�а���һ������ $T$ ($1\le T\le 10^4$)����ʾ����������������

����ÿ��������������һ�а���һ������ $n$ ($2\le n\le 10^5$)����ʾ�����������

�������� $n-1$ �У�ÿ�а����������� $u$ �� $v$ ($1\le u, v\le n$)����ʾ���ӷ��� $u$ �ͷ��� $v$ ��ͨ����

��֤���в��������� $n$ ���ܺͲ����� $2\times 10^5$�����ҷ����ͨ��ʼ�չ���һ������

����ÿ���������������һ�����ֱ�ʾ��ӵ�ͨ������С����������ֻ��� $-1$��

**�������ʽ��**

���һ����������ʾ�𰸡�

���������ڣ�[ChatGPT](https://chatgpt.com/)

```input1
4
2
1 2
4
1 2
2 3
3 4
4
1 2
2 3
2 4
5
1 2
2 3
3 4
3 5

```

```output1
-1
1
-1
2

```

