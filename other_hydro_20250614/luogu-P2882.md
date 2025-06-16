## ��Ŀ����
Farmer John has arranged his N (1 �� N �� 5,000) cows in a row and many of them are facing forward, like good cows. Some of them are facing backward, though, and he needs them all to face forward to make his life perfect.

Fortunately, FJ recently bought an automatic cow turning machine. Since he purchased the discount model, it must be irrevocably preset to turn K (1 �� K �� N) cows at once, and it can only turn cows that are all standing next to each other in line. Each time the machine is used, it reverses the facing direction of a contiguous group of K cows in the line (one cannot use it on fewer than K cows, e.g., at the either end of the line of cows). Each cow remains in the same \*location\* as before, but ends up facing the \*opposite direction\*. A cow that starts out facing forward will be turned backward by the machine and vice-versa.

Because FJ must pick a single, never-changing value of K, please help him determine the minimum value of K that minimizes the number of operations required by the machine to make all the cows face forward. Also determine M, the minimum number of machine operations required to get all the cows facing forward using that value of K.

$N$ ͷţ�ų�һ�� $1 \le N \le 5000$��ÿͷţ������ǰ�������Ϊ��������ţ������ǰ����ũ��ÿ�ο��Խ� $K$ ͷ������ţת�� $1 \le K \le N$����ʹ����������С����Ӧ $K$ ����С�Ĳ������� $M$��$F$ Ϊ��ǰ��$B$ Ϊ����

����һ������������� $K$ �� $M$���ÿո�ֿ���

## �����ʽ
Line 1: A single integer: N


Lines 2..N+1: Line i+1 contains a single character, F or B, indicating whether cow i is facing forward or backward.


## �����ʽ
Line 1: Two space-separated integers: K and M


```input1
7
B
B
F
B
F
B
B
```

```output1
3 3
```

## ��ʾ
For K = 3, the machine must be operated three times: turn cows (1,2,3), (3,4,5), and finally (5,6,7)


