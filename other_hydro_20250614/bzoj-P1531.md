## ��Ŀ����
The Byteotian Bit Bank (BBB) has the largest network of cash dispensers in the whole Byteotia. The BBB have decided to improve their dispensers and have asked you for help. The legal tender in Byteotia are bank notes of denominations $b_1,b_2,\cdots,b_n$. The BBB have concluded that the cash dispensers are to pay every sum in the smallest possible total number of notes.

TaskWrite a programme that:

reads from the standard input the description of the dispenser's notes stock and the sum to be paid off,determines the minimal total number of bank notes sufficient to pay the desired sum off, and finds some way of paying it off as well (using the determined minimal number of notes, of course)writes the result to the standard output.

`Byteotian Bit Bank (BBB)` ӵ��һ���Ƚ��Ļ���ϵͳ�����ϵͳһ���� $n$ ����ֵ��Ӳ�ң���ֵ�ֱ�Ϊ $b_1,b_2,\cdots,b_n$������ÿ��Ӳ�����������ƣ�����������Ҫ�ճ���ֵ $k$��������Ҫ�ö��ٸ�Ӳ��.

## �����ʽ
In the first line of the standard input the number of denominations is written $n$, $1\le n\le 200$. The second line contains $n$ integers $b_1,b_2,\cdots,b_n$, $1\le b_1<b_2<\cdots<b_n\le 20\ 000$, separated by single spaces. The third line contains $n$ integers $c_1,c_2,\cdots,c_n$, $1\le c_i\le 20\ 000$, also separated by single spaces; $c_i$ is the number of banknotes of denomination $b_i$ left in the cash dispenser. In the last, fourth line of input there is one integer $k$ - the sum to be paid off, $1\le k\le 20\ 000$ . For the test data, you are free to assume that the sum $k$ can be paid off in the available banknotes.

��һ��һ������ $n$��

�ڶ��� $n$ ������ $b_i$����ʾ�� $n$ ��Ӳ�ҵ���ֵ��

������ $n$ ������ $c_i$����ʾ�� $n$ ��Ӳ�ҵ�������

������һ������ $k$��

## �����ʽ
The first line of the standard output should contain one integer denoting the minimal total number of bank notes sufficient to pay the sum off $k$. The second line should contain $n$ integers, separated by single spaces, denoting the numbers of notes of subsequent denominations used to pay off the sum $k$. If there are many solutions your programme should write any of them.

��һ��һ����������ʾ������Ҫ���ٸ�Ӳ�ҡ�

�ڶ��� $n$ ����������ʾ�� $i$ ��Ӳ����Ҫ���ٸ���

����ж��ַ������������һ�ּ��ɡ�

## ��������
```plain
3
2 3 5
2 2 1
10
```


## �������
```plain
3
1 1 1
```

## ���ݷ�Χ

���� $100 \%$ �����ݣ�$1 \le n \le 200$��$1 \le b_1 < b_2 < \cdots < b_n \le 2 \times 10^4$��$1 \le c_i,k \le 2 \times 10^4$��