## ��Ŀ����
��¶ŵ��һƬ�����ε�ѩ�أ������������һ��С���ݡ�


## ��Ŀ����
��¶ŵżȻ��õ���һƬ $N\times N$ ��С�������ε�ѩ�أ������������һ����ѩС�ݡ�

����Ƥ�Ģ�Ų���������ռ������أ���Ҫ����Ƭ������ʹ�ñ�ѩ��Ļ�������ש��Ȼ��һ��һ��ش���һ�����ӡ�

��¶ŵ�����ש�ķ�ʽ�������ģ�����վ��ĳ�������ϣ�Ȼ�����ϣ��£����ң����ϣ����£����ϣ�������˸�����֮һ����ǿ���ı�ѩ��Ļ����Ļ��Ӱ�쵽�÷���һ��ֱ����һ���ľ������ڵ����з���

�����ÿ��������һ���䶳�ȣ���ʼΪ $0$������ѩ��ĻӰ��һ�Σ��䶳�� $+1$���䶳�ȵ�����Ϊ $4$��

�ڷ��䵯Ļ�ļ�϶�У���¶ŵ�����������䶳��Ϊ $4$ �ĸ��ӣ��������ѩ�ѵ�һ������һ����ש����СΪ $1\times1\times1$ ���񣩣����ҽ��䶳�����¹��㡣

��¶ŵ��������Щ��ש���Ƿ��ӡ�������ӵĳ��ȡ���Ⱥ�����λ������һ��ʼ���Ѿ��滮���ˣ���������Ը������ȷ�����ӵĸ߶ȡ�

��¶ŵ�������ƻ��ģ������������Ͽ�������һ�������塣

�����ȸ���������ӵ�����ǽ�����Ϊ $1$ �����񣩣��������������λ�ã��ϻ�����һ����Ⱥ͸߶ȷֱ�Ϊ $1$ �� $2$ �Ŀ�λ���ű�ש����Ϊ���š�����Ȼ�����޷�����ǽ�ĹսǴ��������Խ����սǣ���

����ϲ����ʱ�������������ǽ�Ľ��죬��һ������ǽ��������һ�����Ϊ $1$ ������ݶ���ʹ���ӳ�Ϊһ�������ж��ĳ����塣

�ƻ��Ѿ��ǳ�����ˣ�����¶ŵ���ǲ����ģ����������������дһ����������ʱ�����������ʲô������������Ҫ�߱��Ĺ��ܽ���������ϸ���ܡ�

----------------------
ѩ���� $N$ �� $N$ �У�$N\times N$ ��������ɡ����±�� $0$ ��ʼ��Ҳ����˵�����ڵ� $0$ �е� $0$ �У��������ڵ� $N$ �е� $N$ �У�ÿ��������һ���䶳��,��Χ $[0,4]$����ʼΪ $0$��ע�⣬�ռ�����ά�ģ����䶳��ֻ�ǵ�������ԡ�

��¶ŵ�뽫���ӵ����ϽǷ��ڵ� $H_R$�У�$H_C$ �У���ǽҲ�Ƿ��ӵ�һ���֣�������Ͻ�λ�ò�Ӧ���Ƿ��ӵ��ڲ�,������ǽ,������ǽ�Ĺսǣ���

������ӵĳ��ȣ�ƽ����ÿ�У��� $H_X$����ȣ�ƽ����ÿ�У��� $H_Y$������ǽ����֤������ռ�ռ䲻�ᳬ��ѩ�صķ�Χ��

��������ݶ�����¶ŵֻ���ڸ߶� $[0,H_M-1]$ ���ñ�ש��

һ��ʼ����¶ŵһ����שҲû�С�
�����µĽ����У������ø���ͼ����ʾ�⣺
```plain
0000
0000
4x90
0x01
```
���ִ���ǰ�ø��ӵ��䶳�ȡ����λ�ý������棨�߶�Ϊ $0$���ĵط������˱�ש����ô����ĸ $x$ ��ʾ��

������������λ��û�б�ש������λ�����Ϸ��ĸ߿մ��ڱ�ש����ô��Ȼ�����ֱ�ʾ������䶳�ȣ���������ֻ����� $5$���������ʾ��ͼ�п�����һ������ $t\ge5$����ʾ��λ�õ����ǿյģ����ߴ��б�ש���ҵ�����䶳��Ϊ $t-5$��

��һ��������`ICE_BARRAGE R C D S`  
---------------
��ʾ��¶ŵվ�ڵ� $R$ �� $C$ �е�λ�ã����ŷ��� $D$ ������һ��ǿ��Ϊ $S$ �ĵ�Ļ��  
$R,C,D,S\in\mathbf{Z},0\le D\le7,0\le R,C,S<N$��  
������ $0$ ��ʾ�� $(R-1,C)$��$1$ ��ʾ���� $(R-1,C-1)$��   
$2$ ��ʾ�� $(R,C-1)$��$3$ ��ʾ���� $(R+1,C-1)$��  
$4$ ��ʾ�� $(R+1,C)$��$5$ ��ʾ���� $(R+1,C+1)$��  
$6$ ��ʾ�� $(R,C+1)$��$7$ ��ʾ���� $(R-1,C+1)$��  
ǿ��Ϊ $S$ �ĵ�Ļ������ʹ�����ڷ��䷽��ֱ���ϣ�������¶ŵ������ $S$ ������и��ӣ�������վ�ĸ��ӣ������䶳�ȶ� $+1$�������¼������������

1. ���ĳ�������䶳��Ϊ $4$����ô�ø����䶳�Ȳ��䡣
2. �����Ļ����·;�ϣ���һ��λ�õĵ����ϣ��߶�Ϊ $0$���Ѿ����˱�ש�����ǵ�Ļײ������¶ŵ�Ѿ�����һ��ķ��ӣ�����ô��Ļ�����赲���޷�Ӱ�쵽��ש���ڵĸ����Լ���ש���汻��ס�ĸ��ӡ�
3. ��Ļ����ѩ�صĲ��ֺ��Բ��ơ�

���������������Ҫ�������һ�У�`CIRNO FREEZED k BLOCK(S)`  
��������Ļ��ĳ��������䶳�ȳɹ������� $1$����ô��Ϊ�����Ļ��ס�˸÷���

`k` ��ʾ�����Ļ�ܹ���ס�˶��ٷ���

��ͼ�����䵯Ļǰ��ͼ���£�
```plain
00000
00000
00000
000x0
00000
```
ִ�в��� `ICE_BARRAGE 1 1 5 4`����ͼ��Ϊ��
```plain
00000
01000
00100
000x0
00000
```
�����`CIRNO FREEZED 2 BLOCK(S)`  
���ͣ���¶ŵվ�ڵ�һ�е�һ�У�������½Ƿ�����һ��ǿ��Ϊ $4$ �ĵ�Ļ������Ļ�� `x` ���赲��ֻ��Ӱ�쵽 `x` ֮ǰ�ĸ��ӡ�

�ڶ���������`MAKE_ICE_BLOCK`  
-------------------------
��¶ŵ�߱��ͼ�������䶳��Ϊ $4$ �ķ���ÿ����������ռ�һ����ש��Ȼ�����ǵ��䶳�ȹ��㡣 

�����������������Ҫ�����������һ�У�`CIRNO MADE x ICE BLOCK(S),NOW SHE HAS y ICE BLOCK(S)`  
��ʾ��¶ŵ������ $x$ ����ש��Ŀǰ���� $y$ ����ש��  
������¶ŵһ��ʼ�� $0$ ����ש������״̬���£�
```plain
0xxx
0x4x
0x9x
0400
```
ִ�в��� `MAKE_ICE_BLOCK` ���Ϊ
```plain
0xxx
0x0x
0x5x
0000
```
�����`CIRNO MADE 3 ICE BLOCK(S),NOW SHE HAS 3 ICE BLOCK(S)`  
�����ʾ���У������Ѿ������һ���֣�`x` ��ʾǽ��`9` ���λ�õ���û�б�ש�����ߴ��У����Բ³����ţ���������Ψһһ��յء��ŵ�λ�ã��Լ��������һ��λ�õ��䶳�ȶ��ﵽ�� $4$����˿����ռ��� $3$ ���ש���ռ�������λ���䶳�ȶ����㡣

������������`PUT_ICE_BLOCK R C H` 
-----------------
��ʾ�ڵ� $R$ �У��� $C$ �У��߶�Ϊ $H$ �ĵط���һ����ש��$0\le R,C<N,0\le H<H_M$��

���������λ�ø߶�Ϊ $0$�������ש���óɹ�����ô��¶ŵ���ı�ש�������� $1$��

������õ�λ���������棬��λ���䶳�������� $0$��

�����¼�����������ԽС���ȼ�Խ�ߣ�����ֻ������һ�������

������� $1$ �Ļ��ͺ��Ӻ���ģ������� $1$ ��ǰ���²ſ������� $2\cdots\cdots$ �Դ����ơ�

1. ��¶ŵĿǰû���κα�ש���޷����á��������������Ҫ�����`CIRNO HAS NO ICE_BLOCK`
2. ��ש�����ڰ���У��޷����������κα�ש������Ŀ��λ�����б�ש�ˡ�  
�������������Ҫ���һ�У�`BAKA CIRNO,CAN'T PUT HERE`�������Ӵ˴β����������κι�����
3. ��ש�����˹滮���췿�ӵ�����֮�⣬��
$R<H_R$ �� $R>H_R+H_x-1$  
�� $C<H_C$ �� $C>H_C+H_Y-1$�������һ�У�`CIRNO MISSED THE PLACE`  
������¶ŵ�Ŵ��˵ط������㲢������ֹ�����������ש��  
4. ��ש�����˷��ӵ��ڲ�����Ӧ���յĵط���ռ���ˣ���  
$H_R+1\le R\le H_R+H_X-2$ �� $H_C+1\le C\le H_C+H_Y-2$  
���ݶ��ĸ߶ȹ̶�����ǰ�����ǽ�����������ʽ���������Ϊ�Ƿ����˷����ڲ���  
�����һ�У�`CIRNO PUT AN ICE_BLOCK INSIDE THE HOUSE`  
������¶ŵ�Ŵ��˵ط������㲢������ֹ�����������ש��
5. ��ש��������ȷ��λ�ã����ؿ����Ƿ��ס�������ŵĵط���  
�����һ�У�`CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS x ICE_BLOCK(S)`  
`x` ��ʾ�Ź�����ש����¶ŵʣ��ı�ש��

���ĸ�������`REMOVE_ICE_BLOCK R C H` 
---------
��ʾȡ�ߵ� $R$ �У��� $C$ �У��߶�Ϊ $H$ ���ı�ש��  
�����¼�����������ԽС���ȼ�Խ�ߣ�����ֻ������һ�������

������� $1$ �Ļ��ͺ��Ӻ���ģ������� $1$ ��ǰ���²ſ������� $2\cdots\cdots$ �Դ����ơ�

1. Ŀ��λ��û�б�ש�����һ�У�`BAKA CIRNO,THERE IS NO ICE_BLOCK`
2. Ŀ��λ���б�ש�������������ש�����ߺ�������һ����ש�γ���һ�����յĿ顣  
������ġ�����ͼ����`x` ��ʾ��ש��`0` ��ʾ��λ��
```plain
xxxx
x000
x000
x000
```
$\ \ $���������Ͻǵı�ש�󣬵�һ���ұ�������שû�����������γ���һ�����յ���ͨ�飬���������������  
$\ \ $�����ש���ɹ����ߣ���¶ŵ�ı�ש��潫�� $+1$���������е�������ͨ�鶼�������ˤ�鲢��ʧ  
$\ \ $���Ȳ�������ש��棬Ҳ�����ڵ����������κκۼ�����  
$\ \ $���һ�У�`CIRNO REMOVED AN ICE_BLOCK,AND k BLOCK(S) ARE BROKEN`��`k` ��ʾˤ��ı�ש������  
3. ��¶ŵŲ���˱�ש������������ש�����κ�Ӱ�졣    
$\ \ \ $��¶ŵ�ı�ש��� $+1$�����һ�У�`CIRNO REMOVED AN ICE_BLOCK`
    
�����������`MAKE_ROOF` 
--------
�������ֻ�����һ�Σ�����ֻ����Ϊ���һ��������  
�������������¶ŵ�Ѿ�����˱�ѩС�ݵ���ǽ��ֻʣ�ݶ��ˣ�  

һ������£���¶ŵ���������� $H_X\times H_Y$ ����ש�������Ƿ�����ǽ����ߵĸ߶� $+1$ ����һ�㣬  
�γ�һ���ݶ���Ȼ�����Ƴ����ж���ı�ש���������������в�ȱ��ǽ�ڡ�

����Ҫ��˳����ִ���������̣�һ������ĳ���� $\bullet$ ��ʶ�������������ִ�����������˳����̡�

���������֮���������ľ�Ϊһ�������ֻҪ֮ǰû����Ϊ����ĳ������������˳����̣�����Ϊ������һ�������

���ȣ���¶ŵ����һ���Է������ $H_X\times H_Y$ ����ש�������ݶ���

Ϊʲô������أ���ע��һ�㣺���֮ǰ��������ڷ����ڲ��ı�שǡ�ó䵱���ݶ���һ���֣���ô�Ͳ��������λ���ٷű�ש�ˡ����ң����б��ݶ��ߵı�ש��֮����Ϊ����������˷����ⲿ��

ע�⣬���ݶ���ʱ����ܻᴥ�����߶�Ϊ $H_M$ ���Ǹ�ƽ�档

�����ݶ�ǰ�󽫻������������������
- ��¶ŵʣ��ı�ש�����Խ����ݶ������һ�У�`SORRY CIRNO,NOT ENOUGH ICE_BLOCK(S) TO MAKE ROOF`
- ǽ�ڵ���߸߶�С�� $2$ �����񣬻����ڲ���Ч�ռ�С����������  
ǽ�����ڵ�һȦ�����ڲ��ռ䡣�����ڲ���Ч�ռ�ʱ����Ӵ�����õı�ש����Ϊ���ǽ���Ҫ���Ƴ���  
���һ�У�`SORRY CIRNO,HOUSE IS TOO SMALL`

���������������

�˺�������Ϊ��¶ŵ�Ѿ�������ݶ������������Ƴ����ж����ש�ˡ����Ƴ������У���¶ŵ�ᾡ�����ø��ٵı�שˤ�顣���ǽ����ĳ����ש��Ϊ�����˶���ı�ש����Ҫˤ�飬��ô�����Ȳ��ǽ���ϵ��Ǹ���ש��Ȼ�����ǽ�ڲ�ȱʱ���²���������Ȼ��������Ϊ����Ӱ�쵽ǽ�����޲�ȱ�Ķ��ԣ�����������ʧһ����ש���������������һ������ǽ�����Ҳ���ˤ��ı�ש��  
������У�  
`K1 ICE_BLOCK(S) INSIDE THE HOUSE NEED TO BE REMOVED`  
`K2 ICE_BLOCK(S) OUTSIDE THE HOUSE NEED TO BE REMOVED`  
`K1`��ʾ�����ڲ�������õı�ש������`K2`��ʾ�����ⲿ������õı�ש������

���п�������һ�����������
- ��¶ŵ�Ƴ������ж���ı�ש�������Ƴ������У��ݶ������ˡ�  
���һ�У�`SORRY CIRNO,HOUSE IS BROKEN WHEN REMOVING BLOCKS`

���������������

�˺�������Ϊ��¶ŵ�Ѿ��Ƴ������ж���ı�ש�����������ǽ�ڵĲ�ȱ�ˡ�

ǽ���в�ȱ�Ķ����ǣ����˿�Ϊ $1$����Ϊ $2$ �������⣬
�ڷ����ڲ������滹�ܿ�������ȱ�ڡ�

���ĳ����λ����Ҫ��Ϊ�ŵ�һ���֣������ڲ�ȱ�����ҷ���ֻ����һ���š�

���ǽ��û�в�ȱ����Ҫ���������Ҫ�������Ҫ����ǽ���Ƿ��в�ȱ��֮����õ���

��Ĳ����ǣ�ʹ�þ������ٵı�ש������ȷ��λ���ǽ�ڣ�ʹ���ݵ�״̬������ǽ���в�ȱ�Ķ��壨�����ܷ��ö���ı�ש��ͨ���ڵ��������ﵽĿ�ģ����ڴ˶����£�**�����**����������迼���Ľǵ������Ƿ���������Ϊ�ڷ����￴������

���п�������һ�����������
- ��¶ŵʣ��ı�ש�������ǽ�ڵĲ�ȱ��  
���һ�У�`SORRY CIRNO,NOT ENOUGH ICE_BLOCKS TO FIX THE WALL`

���������������

�˺�������Ϊ���ӱ��ɹ������ˣ���ʱ����Ҫ��������������Է��ӽ������ۡ�

���������ôһ������ף���ӵĽ��ɣ�`GOOD JOB CIRNO,SUCCESSFULLY BUILT THE HOUSE`  
1. �����������λ���Ҳ���һ�����Ϊ $1$���߶�Ϊ $2$ ��λ�������š�  
	���һ�У�`HOUSE HAS NO DOOR`��Ȼ����¶ŵ�ᾡ��������ǽ���ϵĲ�ȱ����һ���š�  
    �������һ�У�`DOOR IS OK`
2. ���������һ�б�ʾ�֮ǰǽ�ڵ������̶�  
	2.1. ��֮ǰ�ļ�¼�У�ǽ�ڲ���������Ҫ�޲��������`WALL NEED TO BE FIXED`  
    2.2. ��֮ǰ�ļ�¼�У�ǽ�������������޲��������`WALL IS OK`  
3. ������һ�б�ʾ�Ľǵ������̶ȡ�  
	����ĸ��ǵ������в������ĵط����������`CORNER NEED TO BE FIXED`  
    ����������£������¶ŵʣ��ı�ש�㹻�޸��սǵĿ�ȱ����ô��ֱ�ӻ��޸������ȱ��  
    ��������Ļ��������ٶ��ռ�������ש������ǡ���޸������ȱ��Ȼ���޸������ȱ��  
    ���������`CORNER IS OK`
    
�����������һ�У�`CIRNO FINALLY HAS k ICE_BLOCK(S)`  
`k` ��ʾ��¶ŵ���ʣ��ı�ש��������

��������֮ǰ�ļ�¼�У�ǽ��������ȱ��û��һ��λ����Ҫ����������ⶼ���κζ���ķ��飬û��һ��λ����Ҫ�Ƴ���û�г��ַ���û�ŵ�����������Ľǵ�����Ҳ�����ݶ�ǰ��ȫ��ã�������ͨ���޲����Ƶġ�������ǡ�ÿ�����ĳ��ǽ�������루�������Ϊż�����м���������㣩�����һ�У�   
`CIRNO IS PERFECT!`

## �����ʽ
��һ��һ�������� $N$����ʾѩ�صĴ�С��

�ڶ���һ��������$H_M$����ʾ��¶ŵ���÷�������߶ȡ�

�������ĸ������� $H_R,H_C,H_X,H_Y$����ʾ�������Ͻ�λ�õ��������꣬���ӵĳ����Լ���ȡ�

������һ�������� $M$����ʾ������������

������ $M$ �У�ÿ�б�ʾһ�������������ʽ����Ŀ������

## �����ʽ
����Ŀ�������Ѿ����ܡ�


```input1
8
10
4 0 4 4
63
ICE_BARRAGE 2 1 1 3
ICE_BARRAGE 0 1 3 1
MAKE_ICE_BLOCK
PUT_ICE_BLOCK 3 2 0
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 2 0 6 7
ICE_BARRAGE 3 0 6 7
ICE_BARRAGE 4 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
MAKE_ICE_BLOCK
PUT_ICE_BLOCK 4 0 1
PUT_ICE_BLOCK 4 0 0
PUT_ICE_BLOCK 4 0 1
PUT_ICE_BLOCK 3 0 1
REMOVE_ICE_BLOCK 4 0 1
PUT_ICE_BLOCK 4 2 0
PUT_ICE_BLOCK 6 1 0
PUT_ICE_BLOCK 4 3 0
PUT_ICE_BLOCK 5 3 0
PUT_ICE_BLOCK 6 3 0
PUT_ICE_BLOCK 7 3 0
ICE_BARRAGE 0 1 4 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
MAKE_ICE_BLOCK
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
MAKE_ICE_BLOCK
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
MAKE_ICE_BLOCK
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
ICE_BARRAGE 1 0 6 7
MAKE_ICE_BLOCK
REMOVE_ICE_BLOCK 6 1 0
PUT_ICE_BLOCK 5 0 0
PUT_ICE_BLOCK 6 0 0
PUT_ICE_BLOCK 7 0 0
PUT_ICE_BLOCK 7 1 0
PUT_ICE_BLOCK 7 2 0
PUT_ICE_BLOCK 4 0 1
PUT_ICE_BLOCK 5 0 1
PUT_ICE_BLOCK 6 0 1
PUT_ICE_BLOCK 7 0 1
PUT_ICE_BLOCK 7 1 1
PUT_ICE_BLOCK 7 2 1
PUT_ICE_BLOCK 7 3 1
PUT_ICE_BLOCK 6 3 1
PUT_ICE_BLOCK 5 3 1
PUT_ICE_BLOCK 4 3 1
PUT_ICE_BLOCK 4 2 1
MAKE_ROOF

```

```output1
CIRNO FREEZED 2 BLOCK(S)
CIRNO FREEZED 2 BLOCK(S)
CIRNO MADE 0 ICE BLOCK(S),NOW SHE HAS 0 ICE BLOCK(S)
CIRNO HAS NO ICE_BLOCK
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 7 BLOCK(S)
CIRNO FREEZED 7 BLOCK(S)
CIRNO FREEZED 0 BLOCK(S)
CIRNO MADE 8 ICE BLOCK(S),NOW SHE HAS 8 ICE BLOCK(S)
BAKA CIRNO,CAN'T PUT HERE
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 7 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 6 ICE_BLOCK(S)
CIRNO MISSED THE PLACE
CIRNO REMOVED AN ICE_BLOCK,AND 1 BLOCK(S) ARE BROKEN
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 5 ICE_BLOCK(S)
CIRNO PUT AN ICE_BLOCK INSIDE THE HOUSE
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 3 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 2 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 1 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 0 ICE_BLOCK(S)
CIRNO FREEZED 6 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 7 BLOCK(S)
CIRNO MADE 8 ICE BLOCK(S),NOW SHE HAS 8 ICE BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO MADE 8 ICE BLOCK(S),NOW SHE HAS 16 ICE BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO MADE 8 ICE BLOCK(S),NOW SHE HAS 24 ICE BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO FREEZED 8 BLOCK(S)
CIRNO MADE 8 ICE BLOCK(S),NOW SHE HAS 32 ICE BLOCK(S)
CIRNO REMOVED AN ICE_BLOCK
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 32 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 31 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 30 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 29 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 28 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 27 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 26 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 25 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 24 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 23 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 22 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 21 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 20 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 19 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 18 ICE_BLOCK(S)
CIRNO SUCCESSFULLY PUT AN ICE_BLOCK,NOW SHE HAS 17 ICE_BLOCK(S)
0 ICE_BLOCK(S) INSIDE THE HOUSE NEED TO BE REMOVED
0 ICE_BLOCK(S) OUTSIDE THE HOUSE NEED TO BE REMOVED
GOOD JOB CIRNO,SUCCESSFULLY BUILT THE HOUSE
DOOR IS OK
WALL IS OK
CORNER IS OK
CIRNO FINALLY HAS 1 ICE_BLOCK(S)
CIRNO IS PERFECT!

```

## ��ʾ
����Ϊ $6$ �� **Subtask**��ÿ�� **Subtask** �����ݶ�����һ������������ͬʱ������Ÿ���� **Subtask** ��������  
�� **Subtask #0** ͬʱ���� **Subtask #0~5** ��������  
ÿһ�� **Subtask** �ĵ÷�ȡ���в��Ե����ͷ֡�

**Subtask #0** $20\%$  
��¶ŵֻ�������ѩ��Ļ������������κα�ש��Ҳ����Ƿ���(��ֻ�в���һ�Ͳ�����)��  


**Subtask #1** $10\%$  
��¶ŵ�����Ƴ��Ѿ����õı�ש��

**Subtask #2** $20\%$  
��¶ŵ�������ģ�������û�� `MAKE_ROOF` ������½������ı���(��������£����÷���ĸ߶���Ȼ��С�� $H_M$ ��û�� `MAKE_ROOF` ����)��

**Subtask #3** $20\%$  
��¶ŵ���Ƴ�����ʱ���������,��������κα�שˤ�䡣`MAKE_ROOF` �����Ƴ������שʱ��Ҳ��������ݶ����ݡ�

**Subtask #4** $20\%$  
��¶ŵ��ϲ�����ſ����Ľǵ������Ա�(���ݱ�֤�����п�����Ϊ�ŵ�ǽ�ڿ�ȱ�У���һ�ֿ���ʹ���Ų������Ľǵ�����)�� 

**Subtask #5** $10\%$  
$4\le N\le 16$��$5\le H_M\le 20$��$10\le M\le 10^3$����֤�����ڱ��ݷ�Χ�ڵ����пյ����๹��һ����ͨ�顣

ע�⣺�ж�ǽ���Ƿ��в�ȱʱ����ѡ�Ŀ���λ����������ס���ڵ�ʱ��δ����ա�"�ܿ�����ȱ"�Ե�ʱ�������Ϊ�ж����ݡ�

