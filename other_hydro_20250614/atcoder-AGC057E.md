## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/agc057/tasks/agc057_e

$ H\times\ W $ ���� $ A\ =\ (A_{i,j}) $ ($ 1\leq\ i\leq\ H,\ 1\leq\ j\leq\ W $) �ˌ����ơ��Τβ����򿼤��ޤ���

- **�Х��`��**�����٤Ƥ��Ф�N혤˥��`�Ȥ��롣�Ĥޤꡢ���٤Ƥ� $ i $ �ˌ����� $ A_{i,1},\ldots,A_{i,W} $ ��N혤˥��`�Ȥ��롣
- **�Х��`��**�����٤Ƥ��Ф�N혤˥��`�Ȥ��롣�Ĥޤꡢ���٤Ƥ� $ j $ �ˌ����� $ A_{1,j},\ldots,A_{H,j} $ ��N혤˥��`�Ȥ��롣

$ H\times\ W $ ���� $ B\ =\ (B_{i,j}) $ ���뤨���ޤ����Τ� $ 2 $ ������Ȥ�˜����� $ H\times\ W $ ���� $ A $ �ξt���� $ 998244353 $ �Ǹ�ä��������Ƥ���������

- $ A $ �ˌ������Х��`�ȡ��Х��`�Ȥ򤳤�혤��Фä��Y���� $ B $ ��һ�¤��롣
- $ A $ �ˌ������Х��`�ȡ��Х��`�Ȥ򤳤�혤��Фä��Y���� $ B $ ��һ�¤��롣

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���ޤ���

> $ H $ $ W $ $ B_{1,1} $ $ B_{1,2} $ $ \ldots $ $ B_{1,W} $ $ \vdots $ $ B_{H,1} $ $ B_{H,2} $ $ \ldots $ $ B_{H,W} $

## �����ʽ
�����򜺤������� $ A $ �ξt���� $ 998244353 $ �Ǹ�ä�����������Ƥ���������

## ��Ŀ����
����һ�� $n\times m$��ֵ�� $[0,9]$ �ľ��� $B$����������ж��ٸ���С��ͬ�ľ��� $A$ ��������������

- �ֱ�� $A$ �� **ÿһ��** ��Ԫ�ش�С���������ٷֱ�� $A$ �� **ÿһ��** ��Ԫ�ش�С���������ܹ��õ� $B$��
- �ֱ�� $A$ �� **ÿһ��** ��Ԫ�ش�С���������ٷֱ�� $A$ �� **ÿһ��** ��Ԫ�ش�С���������ܹ��õ� $B$��

$1\le n,m\le 1500$���𰸶� 998244353 ȡģ��

```input1
2 2
0 0
1 2
```

```output1
4
```

```input2
3 3
0 1 3
2 4 7
5 6 8
```

```output2
576
```

```input3
3 5
0 0 0 1 1
0 0 1 1 2
0 1 1 2 2
```

```output3
10440
```

```input4
1 7
2 3 3 6 8 8 9
```

```output4
1260
```

## ��ʾ
### �Ƽs

- $ 1\leq\ H,\ W\leq\ 1500 $
- $ 0\leq\ B_{i,j}\leq\ 9 $
- ����� $ 1\leq\ i\leq\ H $ ����� $ 1\leq\ j\leq\ W\ -\ 1 $ �ˌ����� $ B_{i,j}\leq\ B_{i,j+1} $
- ����� $ 1\leq\ j\leq\ W $ ����� $ 1\leq\ i\leq\ H\ -\ 1 $ �ˌ����� $ B_{i,j}\leq\ B_{i+1,j} $
- ��������낎�Ϥ��٤�����

### Sample Explanation 1

�����򜺤������ФϴΤ� $ 4 $ �ĤǤ���$ \begin{pmatrix}0&amp;0\\1&amp;2\end{pmatrix} $, $ \begin{pmatrix}0&amp;0\\2&amp;1\end{pmatrix} $, $ \begin{pmatrix}1&amp;2\\0&amp;0\end{pmatrix} $, $ \begin{pmatrix}2&amp;1\\0&amp;0\end{pmatrix} $. �����С�$ \begin{pmatrix}2&amp;1\\0&amp;0\end{pmatrix} $ �������򜺤������ȤϴΤΤ褦�˴_������ޤ��� - �Х��`�ȡ��Х��`�Ȥ򤳤�혤��Ф����ϣ�$ \begin{pmatrix}2&amp;1\\0&amp;0\end{pmatrix}\to\ \begin{pmatrix}1&amp;2\\0&amp;0\end{pmatrix}\ \to\ \begin{pmatrix}0&amp;0\\1&amp;2\end{pmatrix} $. - �Х��`�ȡ��Х��`�Ȥ򤳤�혤��Ф����ϣ�$ \begin{pmatrix}2&amp;1\\0&amp;0\end{pmatrix}\to\ \begin{pmatrix}0&amp;0\\2&amp;1\end{pmatrix}\ \to\ \begin{pmatrix}0&amp;0\\1&amp;2\end{pmatrix} $.

### Sample Explanation 2

������ $ \begin{pmatrix}5&amp;7&amp;6\\3&amp;0&amp;1\\4&amp;8&amp;2\end{pmatrix} $ �������򜺤����ޤ������Τ��ȤϴΤΤ褦�˴_������ޤ��� - �Х��`�ȡ��Х��`�Ȥ򤳤�혤��Ф����ϣ�$ \begin{pmatrix}5&amp;7&amp;6\\3&amp;0&amp;1\\4&amp;8&amp;2\end{pmatrix}\to\ \begin{pmatrix}5&amp;6&amp;7\\0&amp;1&amp;3\\2&amp;4&amp;8\end{pmatrix}\ \to\ \begin{pmatrix}0&amp;1&amp;3\\2&amp;4&amp;7\\5&amp;6&amp;8\end{pmatrix} $. - �Х��`�ȡ��Х��`�Ȥ򤳤�혤��Ф����ϣ�$ \begin{pmatrix}5&amp;7&amp;6\\3&amp;0&amp;1\\4&amp;8&amp;2\end{pmatrix}\to\ \begin{pmatrix}3&amp;0&amp;1\\4&amp;7&amp;2\\5&amp;8&amp;6\end{pmatrix}\ \to\ \begin{pmatrix}0&amp;1&amp;3\\2&amp;4&amp;7\\5&amp;6&amp;8\end{pmatrix} $.

