## ��Ŀ����
Captain Bovidian is on an adventure to rescue her crew member, Doctor Beefalo.  Like all great adventures, this story plays out in a two dimensional N by M grid (1 <= N, M <= 500), representing a side view of the captain's world.  Some grid cells are empty while others are blocked and cannot be traversed.

Unfortunately, Captain Bovidian cannot jump.  She must obey the following rules of physics while traversing her world.

1) If there is no cell directly underneath Captain Bovidian (that is, if she is at the edge of the grid), then she flies out into space and fails her mission.

2) If the cell directly underneath Captain Bovidian is empty, then she falls into that cell.

3) Otherwise:

a) Captain Bovidian may move left or right if the corresponding cell exists and is empty.

b) Or, Captain Bovidian may flip the direction of gravity.

When Captain Bovidian changes the direction of gravity, the cell that's 'underneath' her (as mentioned in rules 1 and 2) toggles between the cell with one higher row index and the cell with one lower row index (the first row in the input has index 1, and the last row has index N). Initially, the cells with one higher row index are underneath Captain Bovidian.

Doctor Beefalo is lost somewhere in this world.  Help Captain Bovidian arrive at her cell using the least number of gravity flips as possible.  If it is impossible to reach Doctor Beefalo, please output -1.


Bovidian ���������������Ĵ�Ա��Beefalo ��ʿ��

������ΰ���ð�չ���һ�����������Ҳ�Ƿ�����һ��2Dƽ���ϵġ���

���ƽ����M\*N�ĸ�����ɵ����񣬴����Ŵ����������һ������ͼ��

��Щ�����ǿյģ���һЩ����ʵ�ĵģ����Ҳ���ֱ��ͨ����

�ܲ��ҵ��ǣ�������������������������������������������

1��������������·�û�з��飨���仰˵����ʹ����������ı�Ե������ô���ͻ���������У�ͬʱ��ζ��ð��ʧ�ܡ�

2��������������·��ķ����ǿյģ���ô���ͻ����������飬

3���ڲ�����1����2��������£�����������һ�µ����飺

a) ������(���ұߣ��ķ����ǿյģ���ô�������ߵ��Ǹ����ӡ�

b�������Է�ת�����ķ���

�������ı䷭ת�����ķ���ʱ�����Ǿ͸ı䴬�����·����Ķ��塣

���·����Ķ���ֻ��������

(A)�ȴ���λ�����ڵķ�����б�Ÿ���ĸ��ӣ�

(B)�ȴ���λ�����ڵķ�����б�Ÿ�С�ĸ���,

һ��ʼ��ʱ�򣬡��·����Ķ����Ǳȴ���λ�����ڷ�����б�Ÿ���ĸ��ӡ�

Beefalo��ʿ����ʧ����������е�ĳһ�����������������㵽�ﲩʿ�ĵط���

������Ե�������������Ҫ�ķ�ת�����Ĵ�����


��������Ե�������-1


## �����ʽ
��1�������������� N,M

��2�е�N+1���У���i+1�����Ǵ���������ĵ�i�С�ÿ����M���ַ���

����","������һ���յĸ��ӣ�"#"������һ��ʵ�ĵĸ��ӣ�"C"�����Ŵ�����λ�ã�"D"�����Ų�ʿ��λ�á�


## �����ʽ
һ�У����һ��������

����������Ե�������������Ҫ�ķ�ת�����Ĵ�����

��������Ե�������-1


```input1
5 5
#####
#...#
#...D
#C...
##.##
```

```output1
3
```

## ��ʾ
������ͣ�

���ȣ������ڣ�4,2������������ת���������2,2��

�������������ߵ���2,4�����������ڶ��η�ת���������4,4��

Ȼ�������������ߵ���4,5��������ڷ�תһ�����������ﲩʿ���ڵģ�3,5��


