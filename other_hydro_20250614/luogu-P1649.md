## ��Ŀ����
Consider an N x N (1 <= N <= 100) square field composed of 1

by 1 tiles. Some of these tiles are impassible by cows and are marked with an 'x' in this 5 by 5 field that is challenging to navigate:

```cpp
. . B x . 
. x x A . 
. . . x . 
. x . . . 
. . x . . 
```
Bessie finds herself in one such field at location A and wants to move to location B in order to lick the salt block there.  Slow, lumbering creatures like cows do not like to turn and, of course, may only move parallel to the edges of the square field. For a given field, determine the minimum number of ninety degree turns in any path from A to B. The path may begin and end with Bessie facing in any direction. Bessie knows she can get to the salt lick.



## �����ʽ
Line 1: A single integer: N

Lines 2..N + 1: Line i+1 represents row i of the field with N characters as above (i.e., '.', 'x', 'A', and 'B'); no spaces are present on a line


## �����ʽ
Line 1: A single integer, the minimum number of turns the cow must make in a traversal

## ��Ŀ����
$N\times N\ (1\le N\le 100)$ �����У�$\verb!x!$ ��ʾ�������ߵĸ��ӣ�$\verb!.!$ ��ʾ�������ߵĸ��ӡ����ź��֣��ʶ�����ת�䡣����Ҫ�� $A$ ���ߵ� $B$ �㣬��������Ҫת $90$ ������ٴΣ�

```input1
3
. x A
. . .
B x .
```

```output1
2
```

## ��ʾ
ֻ�������������ĸ��������ߣ����Ҳ����߳���Щ����֮�⡣��ʼ�ͽ���ʱ�ķ���������⡣

### ���ݷ�Χ��Լ��

����ȫ�����ݣ���֤ $2\le N\le 100$��


