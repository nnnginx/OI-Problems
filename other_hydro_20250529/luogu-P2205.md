## ��Ŀ����
Farmer John has devised a brilliant method to paint the long fence next to his barn (think of the fence as a one-dimensional number line).  He simply attaches a paint brush to his favorite cow Bessie, and then retires to drink a cold glass of water as Bessie walks back and forth across the fence, applying paint to any segment of the fence that she walks past.

Bessie starts at position 0 on the fence and follows a sequence of N moves (1 <= N <= 100,000).  Example moves might be "10 L", meaning Bessie moves 10 units to the left, or "15 R", meaning Bessie moves 15 units to the right.  Given a list of all of Bessie's moves, FJ would like to know what area of the fence gets painted with at least K coats of paint.  Bessie will move at most 1,000,000,000 units away from the origin during her walk.



Farmer John �����һ����ţ���Եĳ�ΧǽͿɫ�ĺ÷�������Ϊ�˼���������ǰ�Χǽ����һά�����ᣬÿһ����λ���ȴ���һ��դ����

��ֻ�Ǽ򵥵İ�ˢ��պ�����ϣ�ϵ������ϲ������ţBessie�ϣ�Ȼ����Bessie���صؾ���Χǽ���Լ�����һ�Ժ�һ���������ˮ��������-\_-|||) 

Bessie ����������Χǽ���ᱻͿ��һ�����ϡ�Bessie��Χǽ�ϵ�λ��0���������������N���ƶ�(1 <= N <= 100,000)������˵����10 L������˼����Bessie�����ƶ���10����λ���ٱ���˵��15 R������˼����Bessie�����ƶ���15����λ��

����һϵ��Bessie�ƶ����嵥��FJ ��֪���ж��ٿ�դ��Ϳ��������K��Ϳ�ϡ�ע�⣺Bessie�����ƶ�����ԭ��1,000,000,000��λԶ�ĵط���


## �����ʽ
\* ��1�У� ���������� N K

\* ��2...N+1 �У� ÿһ�ж�������Bessie��һ���ƶ��� ������˵ ��15 L"��


## �����ʽ
\* һ��������������Ϳ��K��Ϳ�ϵ�դ����

��ע�⣺��������һ��Ҫ������з��������WA��


```input1
6 2 
2 R 
6 L 
1 R 
8 L 
1 R 
2 R 
```

```output1
6
```

## ��ʾ
PS1����Դ��usaco jan silver P01 �뿴ԭ������http://www.usaco.org/index.php?page=viewproblem2&cpid=226��

PS2����������Ҳ��������http://www.usaco.org/index.php?page=jan13problems�����أ������Կ�����⣨������Ӣ�ĵ�:-D��

PS3:����з�����������Ŀ�Ĳ���⣬�������ʴ�������Ե�˵��


