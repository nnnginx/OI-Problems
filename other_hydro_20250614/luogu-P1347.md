## ��Ŀ����
һ����ͬ��ֵ��������������ָ����һ��������Ԫ��������������У����磬һ����������� $A,B,C,D$ ��ʾ $A<B,B<C,C<D$����������У����ǽ�����һϵ������ $A<B$ �Ĺ�ϵ����Ҫ�����ж��Ƿ��ܹ�������Щ��ϵȷ��������е�˳��

## �����ʽ
��һ�������������� $n,m$��$n$ ��ʾ��Ҫ�����Ԫ��������$2\leq n\leq 26$���� $1$ �� $n$ ��Ԫ�ؽ��ô�д�� $A,B,C,D,\dots$ ��ʾ��$m$ ��ʾ������������ $A<B$ �Ĺ�ϵ��������

�������� $m$ �У�ÿ���� $3$ ���ַ����ֱ�Ϊһ����д��ĸ��һ�� `<` ���ţ�һ����д��ĸ����ʾ����Ԫ��֮��Ĺ�ϵ��


## �����ʽ
������ǰ $x$ ����ϵ����ȷ���� $n$ ��Ԫ�ص�˳�� `yyy..y`���� `ABC`�������

`Sorted sequence determined after xxx relations: yyy...y.`

������ǰ $x$ ����ϵ�����ִ���ì�ܣ��� $A<B,B<C,C<A$�������

`Inconsistency found after x relations.`

�������� $m$ ����ϵ�޷�ȷ���� $n$ ��Ԫ�ص�˳�����

`Sorted sequence cannot be determined.`

����ʾ��ȷ�� $n$ ��Ԫ�ص�˳��󼴿ɽ������򣬿��Բ��ÿ���ȷ��˳��֮�����ì�ܵ������


```input1
4 6
A<B
A<C
B<C
C<D
B<D
A<B

```

```output1
Sorted sequence determined after 4 relations: ABCD.
```

```input2
3 2
A<B
B<A
```

```output2
Inconsistency found after 2 relations.
```

```input3
26 1
A<Z
```

```output3
Sorted sequence cannot be determined.
```

## ��ʾ
$2 \leq n \leq 26,1 \leq m \leq 600$��

