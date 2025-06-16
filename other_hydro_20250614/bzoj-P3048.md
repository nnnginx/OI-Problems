## ��Ŀ����

Farmer John's  $ n $  cows are lined up in a row. Each cow is identified by an integer "breed ID" in the range  $ 0...1\times 10^9 $ ; the breed ID of the ith cow in the lineup is  $ B(i) $ . Multiple cows can share the same breed ID. FJ thinks that his line of cows will look much more impressive if there is a large contiguous block of cows that all have thesame breed ID. In order to create such a block, FJ chooses up to K breed IDs and removes from his lineup all the cows having those IDs. Please help FJ figure out the length of the largest consecutive block of cows with the same breed ID that he can create by doing this.

����һ������Ϊ $ n $ ����Ȼ�����У�����ÿһ������С�ڵ��� $ 1\times 10^9 $�����ڸ���һ�� $ k $����ʾ��������ɾȥ $ k $ ��������������ͬ�����ֱ���Ϊһ����������������������е�������ȵ����������б������������У�����������ͨ��ɾ��ʹ�ø������е���������о�������

## �����ʽ

Line 1: Two space-separated integers:  $ n $  and  $ k $.
Lines 2..1+N: Line i+1 contains the breed ID $ B(i) $.

## �����ʽ

Line 1: The largest size of a contiguous block of cows with identical breed IDs that FJ can create.

## ��������

```
9 1
2
7
3
7
7
3
7
5
7
```

## �������

```
4
```

## ��ʾ

����Ϊ9�����У����ֻ��ɾȥ $ 1 $ ������

��ɾ����������г���Ϊ $ 2 $ ��

ɾȥһ���� $ 3 $ �����б�� $ 2,7,7,7,7,5,7 $ ����������г���Ϊ $ 4 $ .��˴�Ϊ $ 4 $ .

## ���ݹ�ģ��Լ��

���� $100\%$ �����ݣ�$  1 \leq n \leq 1\times 10^5  $��

## ��Ŀ��Դ

Gold

