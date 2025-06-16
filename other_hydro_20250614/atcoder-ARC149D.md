## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/arc149/tasks/arc149_d

$ N $ ���Υ��ޤ���ֱ���Ϥ��������ˤ��ä���Ƥ��ޤ���$ i $ ��Ŀ�Υ��ޤ����� $ X_i $ ���ä���Ƥ��ޤ���

�����Υ��ޤ򣬴ΤΤ褦�� $ M $ ���ƄӤ����ޤ���

- $ i $ ��Ŀ�β����Ǥϣ������� $ D_i $ ���뤨��죬�����ޤ�ΤΤ褦���ƄӤ����룮
  - ���ˤ�ؓ�������Ǥ���褦�ʥ��ޤϣ����η���˾��x $ D_i $ �M���λ�ä��ƄӤ����룮
  - ���ˤ� $ 0 $ �Ǥ���褦�ʥ��ޤτӤ����ʤ���
  - ���ˤ����������Ǥ���褦�ʥ��ޤϣ�ؓ�η���˾��x $ D_i $ �M���λ�ä��ƄӤ����룮

�����ޤ�ԭ��˵��_���뤫�񤫤��ж����Ƥ���������ԭ��˵��_������Ϥˤϣ��Ϥ����ԭ��˵��_����Τ��λ�Ŀ���ƄӤˤ���Τ���������Ƥ���������ԭ��˵��_���ʤ����Ϥˤϣ�$ M $ �ؤ��ƄӤ����٤ƽK�ˤ����Ȥ������ˤ�������Ƥ���������

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���ޤ���

> $ N $ $ M $ $ X_1 $ $ \ldots $ $ X_N $ $ D_1 $ $ \ldots $ $ D_M $

## �����ʽ
$ N $ �г������Ƥ���������$ i $ ��Ŀ�ˤϣ�$ i $ ��Ŀ�Υ��ޤˌ����������¤����٤���ʽ�ǳ������Ƥ���������

���ޤ�ԭ��˵��_������Ϥˤϣ��Ϥ����ԭ��˵��_����Τ� $ x $ ��Ŀ���ƄӤǤ���Ȥ���

> Yes $ x $

�ȳ������Ƥ������������ޤ�ԭ��˵��_���ʤ����Ϥˤϣ�$ M $ �ؤ��ƄӤ����٤ƽK�ˤ����Ȥ������ˤ� $ x $ �Ǥ���Ȥ���

> No $ x $

�ȳ������Ƥ���������

## ��Ŀ����
����һ�����ᣬ������ $n$ ���� $x_1,x_2,��,x_n$ ������Ҫ��ÿһ������� $M$ ���ƶ����������£�\
����ÿ�� $x_i$ :\
�������� $>0$���򸺷����ƶ� $D$ ����λ��\
�������� $=0$��ֹͣ�ƶ���\
�������� $<0$�����������ƶ� $D$ ����λ��

����Ҫ�ж�ÿ�����Ƿ�ᵽ��ԭ�㣬\
�ǣ���� "Yes" ��Ȼ�������ʹ���˼����ƶ���\
����� "No" ��Ȼ������� $M$ ���ƶ�������ꡣ

```input1
6 4
2 4 6 8 10 12
8 2 5 7
```

```output1
No -6
No -4
Yes 2
Yes 1
Yes 2
No 4
```

## ��ʾ
### �Ƽs

- $ 1\leq\ N\leq\ 3\times\ 10^5 $
- $ 1\leq\ M\leq\ 3\times\ 10^5 $
- $ 1\leq\ X_1\ <\ \cdots\ <\ X_N\ \leq\ 10^6 $
- $ 1\leq\ D_i\ \leq\ 10^6 $

### Sample Explanation 1

�����ޤ����ˤϴΤΤ褦�ˉ仯���ޤ��� - $ 1 $ ��Ŀ�Υ��ޣ�$ \phantom{0}2\quad\ \longmapsto\ \quad\ -6\quad\ \longmapsto\ \quad\ -4\quad\ \longmapsto\ \quad\ \phantom{-}1\ \quad\ \longmapsto\ \quad\ -6 $. - $ 2 $ ��Ŀ�Υ��ޣ�$ \phantom{0}4\ \quad\ \longmapsto\ \quad\ -4\quad\ \longmapsto\ \quad\ -2\ \quad\ \longmapsto\ \quad\ \phantom{-}3\ \quad\ \longmapsto\ \quad\ -4 $. - $ 3 $ ��Ŀ�Υ��ޣ�$ \phantom{0}6\ \quad\ \longmapsto\ \quad\ -2\quad\ \longmapsto\ \quad\ \phantom{-}0\ \quad\ \longmapsto\ \quad\ \phantom{-}0\ \quad\ \longmapsto\ \quad\ \phantom{-}0 $. - $ 4 $ ��Ŀ�Υ��ޣ�$ \phantom{0}8\ \quad\ \longmapsto\ \quad\ \phantom{-}0\quad\ \longmapsto\ \quad\ \phantom{-}0\ \quad\ \longmapsto\ \quad\ \phantom{-}0\ \quad\ \longmapsto\ \quad\ \phantom{-}0 $. - $ 5 $ ��Ŀ�Υ��ޣ�$ 10\ \quad\ \longmapsto\ \quad\ \phantom{-}2\quad\ \longmapsto\ \quad\ \phantom{-}0\ \quad\ \longmapsto\ \quad\ \phantom{-}0\ \quad\ \longmapsto\ \quad\ \phantom{-}0 $. - $ 6 $ ��Ŀ�Υ��ޣ�$ 12\ \quad\ \longmapsto\ \quad\ \phantom{-}4\quad\ \longmapsto\ \quad\ \phantom{-}2\ \quad\ \longmapsto\ \quad\ -3\ \quad\ \longmapsto\ \quad\ \phantom{-}4 $.

