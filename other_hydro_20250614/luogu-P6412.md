## ��Ŀ����
������һ�� $1\sim n$ ������ $a$���������е�Ԫ�����ηŽ�һ�� BST ��� BST �в��뺯����ִ�д�����

**ע�⣺��һ�����Ѿ���Ϊ BST �ĸ���**

������޷��������˵�Ļ���������һ��α���룺

```
insert( number x, node n )
    c+1;
    if x is less than the number in node n
        if n has no left child
            create a new node with the number x and set it to be the left child of node n
     else
         insert(x, left child of node n)
     else (x is greater than the number in node n)
         if n has no right child
             create a new node with the number x and set it to be the right child of node n
         else
             insert(x, right child of node n) 
```
����Ҫ��ľ�������� insert ����ÿ����һ�κ� $c$ ��ֵ��

**�ٴ�ע�⣺��һ�����Ѿ���Ϊ BST �ĸ���**

## �����ʽ
��һ�У�һ������ $n$����ʾ���� $a$ �ĳ��ȡ�

������ $n$ �У�ÿ��һ���������� $i$ ��Ϊ $a_i$��

## �����ʽ
�� $n$ �У�һ��һ����������ʾ����� insert ����ÿ����һ�κ� $c$ ��ֵ��

```input1
4
1
2
3
4 

```

```output1
0
1
3
6

```

```input2
5
3
2
4
1
5 

```

```output2
0
1
2
4
6 
```

```input3
8
3
5
1
6
8
7
2
4 

```

```output3
0
1
2
4
7
11
13
15 
```

## ��ʾ
#### ���ݷ�Χ������
- ���� $50\%$ �����ݣ���֤ $n\le 10^3$��
- ���� $100\%$ �����ݣ���֤ $1\le n\le 3\times 10^5$��$1\le a_i\le n$��$a_i$ ������ͬ��
#### ˵��
�������� [Croatian Open Competition in Informatics 2008/2009](https://hsin.hr/coci/archive/2008_2009) [Contest #3](https://hsin.hr/coci/archive/2008_2009/contest3_tasks.pdf) T5 BST�� 

