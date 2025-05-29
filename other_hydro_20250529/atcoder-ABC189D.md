## ��Ŀ����
[problemUrl]: https://atcoder.jp/contests/abc189/tasks/abc189_d

$ N $ ���������� $ S_1,\ldots,S_N $ ���뤨���ޤ����������Ф� `AND` �ޤ��� `OR` �Ǥ���

���� $ \text{True} $ �ޤ��� $ \text{False} $ �Ǥ���褦�� $ N+1 $ ���Ή����νM $ (x_0,\ldots,x_N) $ �Ǥ��äơ� ���¤Τ褦��Ӌ����Фä��H�ˡ�$ y_N $ �� $ \text{True} $ �Ȥʤ�褦�ʤ�Τ΂��������Ƥ���������

- $ y_0=x_0 $
- $ i\geq\ 1 $ �ΤȤ���$ S_i $ �� `AND` �ʤ� $ y_i=y_{i-1}\ \land\ x_i $��$ S_i $ �� `OR` �ʤ� $ y_i=y_{i-1}\ \lor\ x_i $

$ a\ \land\ b $ �� $ a $ �� $ b $ ��Փ��e�����$ a\ \lor\ b $ �� $ a $ �� $ b $ ��Փ��ͤ���ޤ���

## �����ʽ
���������¤���ʽ�ǘ˜����������뤨���롣

> $ N $ $ S_1 $ $ \vdots $ $ S_N $

## �����ʽ
�𤨤�������衣

## ��Ŀ����
### ��Ŀ����

�� $n$ ���ַ��� `AND` �� `OR`������ $n + 1$ ��ֵ��ÿ��ֵ�� `TRUE` �� `FALSE`�������ж����ַ�������ʹ������ʽ���Ľ���� `TRUE`�����ʽ�Ľ�����ǽ��� $n$ ���ַ�����˳����� $n + 1$ ��ֵ֮�䣬�������Ҽ��㡣

$1\leq n\leq 60$��

```input1
2
AND
OR
```

```output1
5
```

```input2
5
OR
OR
OR
OR
OR
```

```output2
63
```

## ��ʾ
### �Ƽs

- $ 1\ \leq\ N\ \leq\ 60 $
- $ S_i $ �� `AND` �ޤ��� `OR`

### Sample Explanation 1

������ $ (x_0,x_1,x_2)=(\text{True},\text{False},\text{True}) $ �ΤȤ� - $ y_0=x_0=\text{True} $ - $ y_1=y_0\ \land\ x_1\ =\ \text{True}\ \land\ \text{False}=\text{False} $ - $ y_2=y_1\ \lor\ x_2\ =\ \text{False}\ \lor\ \text{True}=\text{True} $ �Ȥʤꡢ$ y_2 $ �� $ \text{True} $ �ˤʤ�ޤ��� $ y_2 $ �� $ \text{True} $ �Ȥʤ�褦�� $ (x_0,x_1,x_2) $ �νM�ߺϤ碌�ϡ� - $ (\text{True},\text{True},\text{True}) $ - $ (\text{True},\text{True},\text{False}) $ - $ (\text{True},\text{False},\text{True}) $ - $ (\text{False},\text{True},\text{True}) $ - $ (\text{False},\text{False},\text{True}) $ �� $ 5 $ ͨ���ȫ�ƤǤ���

### Sample Explanation 2

ȫ�Ƥ� $ \text{False} $ �ΤȤ������ $ 2^6-1 $ ͨ��� $ y_5 $ �� $ \text{True} $ �ˤʤ�ޤ���

