## Description

<div><p>���ѧ��ާ���ڧ� ��ݧ֧է���ڧ� �ܧ�� �����ڧ��ӧܧ� ��ݧڧ�ߧڧ֧� �ߧ� ��٧��ܧ� Python: </p><pre class="lstlisting"><code class="prettyprint">def sort(a):
  n = len(a)
  b = [0 for i in range(n)]
  log = []

  def mergeSort(l, r):
    if r - l &lt;= 1:
      return
    m = (l + r) &gt;&gt; 1
    mergeSort(l, m)
    mergeSort(m, r)
    i, j, k = l, m, l
    while i &lt; m and j &lt; r:
      if a[i] &lt; a[j]:
        log.append('0')
        b[k] = a[i]
        i += 1
      else:
        log.append('1')
        b[k] = a[j]
        j += 1
      k += 1
    while i &lt; m:
      b[k] = a[i]
      i += 1
      k += 1
    while j &lt; r:
      b[k] = a[j]
      j += 1
      k += 1
    for p in range(l, r):
      a[p] = b[p]

  mergeSort(0, n)
  return "".join(log)
</code></pre><p>���ѧ� �ާ�اߧ� �٧ѧާ֧�ڧ��, ����� �ܧ�� �ڧ���ݧ�٧�֧� �ݧ�ԧڧ��ӧѧߧڧ�&nbsp;�� �ӧѧاߧ֧ۧ�ڧ� �ڧߧ����ާ֧ߧ� ��ѧ٧�ѧҧ��ܧ�.</p><p>����ѧ��ڧ� ��ѧ٧�ѧҧ���ڧ� ������ߧ�ѧܧ�� ���ѧ�� ��ԧ֧ߧ֧�ڧ��ӧѧ� ��֧�֧��ѧߧ�ӧܧ� $a$ (�ާѧ��ڧ� �ڧ� $n$ ��ѧ٧ݧڧ�ߧ��� ��֧ݧ��� ��ڧ�֧� ��� $1$ �է� $n$), �էѧ� �֧� �ߧ� �ӧ��� ���ߧܧ�ڧ� <span class="tex-font-style-tt">sort</span> �� ���ݧ��ڧ� �ߧ� �ӧ����է� �����ܧ� $s$. ���� ��ݧ֧է���ڧ� �է֧ߧ� �����ܧ� $s$ ���ѧ�� �ߧѧ�ק�, �� ��֧�֧��ѧߧ�ӧܧ� $a$ ����֧��ݧѧ��. </p><p>���ѧ�� ����֧� �ӧ����ѧߧ�ӧڧ�� �ݧ�ҧ�� ��֧�֧��ѧߧ�ӧܧ� $a$ ��ѧܧ��, ���� �ӧ��٧�� ���ߧܧ�ڧ� <span class="tex-font-style-tt">sort</span> ��� �ߧ֧� �էѧ�� ��� �ا� �����ܧ� $s$. ����ާ�ԧڧ�� �֧ާ�!</p></div><div class="input-specification"><p>���ӧ�� ���է֧�اڧ� �ߧ֧������ �����ܧ� $s$, ���������� �ڧ� ��ڧާӧ�ݧ�� <span class="tex-font-style-tt">0</span> �� <span class="tex-font-style-tt">1</span>. </p><p><span class="tex-font-style-bf">�� ����� �ӧ֧��ڧ� �٧ѧէѧ��</span> �էݧ� �ݧ�ҧ�ԧ� ��֧��� ����֧��ӧ�֧� ��֧�֧��ѧߧ�ӧܧ� �էݧڧߧ� $16$, ��է�ӧݧ֧�ӧ�����ѧ� ���ݧ�ӧڧ�. ���֧� �ߧ� �ާ֧ߧ֧�, �ӧѧ� ���ӧ֧� �ާ�ا֧� �ڧާ֧�� �ݧ�ҧ�� �էݧڧߧ�, �� ���� ��ڧ�ݧ� ���ݧڧ�ߧ�� ��� $16$.</p></div><div class="output-specification"><p>�� ��֧�ӧ�� �����ܧ� �ӧ��ӧ֧էڧ�� ��֧ݧ�� ��ڧ�ݧ� $n$&nbsp;�� �էݧڧߧ� ��֧�֧��ѧߧ�ӧܧ�.</p><p>���� �ӧ����� �����ܧ� �ӧ��ӧ֧էڧ�� $n$ ��ѧ٧ݧڧ�ߧ��� ��֧ݧ��� ��ڧ�֧� $a_0, a_1, \ldots, a_{n-1}$ ($1 \le a_i \le n$)&nbsp;�� ��ݧ֧ާ֧ߧ�� ��֧�֧��ѧߧ�ӧܧ�.</p><p>����ݧ� ����֧��ӧ�֧� �ߧ֧�ܧ�ݧ�ܧ� �ӧѧ�ڧѧߧ��� ���ӧ֧��, �ӧ��ӧ֧էڧ�� �ݧ�ҧ�� �ڧ� �ߧڧ�.</p></div>

## Input

<p>���ӧ�� ���է֧�اڧ� �ߧ֧������ �����ܧ� $s$, ���������� �ڧ� ��ڧާӧ�ݧ�� <span class="tex-font-style-tt">0</span> �� <span class="tex-font-style-tt">1</span>. </p><p><span class="tex-font-style-bf">�� ����� �ӧ֧��ڧ� �٧ѧէѧ��</span> �էݧ� �ݧ�ҧ�ԧ� ��֧��� ����֧��ӧ�֧� ��֧�֧��ѧߧ�ӧܧ� �էݧڧߧ� $16$, ��է�ӧݧ֧�ӧ�����ѧ� ���ݧ�ӧڧ�. ���֧� �ߧ� �ާ֧ߧ֧�, �ӧѧ� ���ӧ֧� �ާ�ا֧� �ڧާ֧�� �ݧ�ҧ�� �էݧڧߧ�, �� ���� ��ڧ�ݧ� ���ݧڧ�ߧ�� ��� $16$.</p>

## Output

<p>�� ��֧�ӧ�� �����ܧ� �ӧ��ӧ֧էڧ�� ��֧ݧ�� ��ڧ�ݧ� $n$&nbsp;�� �էݧڧߧ� ��֧�֧��ѧߧ�ӧܧ�.</p><p>���� �ӧ����� �����ܧ� �ӧ��ӧ֧էڧ�� $n$ ��ѧ٧ݧڧ�ߧ��� ��֧ݧ��� ��ڧ�֧� $a_0, a_1, \ldots, a_{n-1}$ ($1 \le a_i \le n$)&nbsp;�� ��ݧ֧ާ֧ߧ�� ��֧�֧��ѧߧ�ӧܧ�.</p><p>����ݧ� ����֧��ӧ�֧� �ߧ֧�ܧ�ݧ�ܧ� �ӧѧ�ڧѧߧ��� ���ӧ֧��, �ӧ��ӧ֧էڧ�� �ݧ�ҧ�� �ڧ� �ߧڧ�.</p>

## Samples

```input1
00000000000000000000000000000000
```

```output1
16
1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16
```






```input2
11111111111111111111111111111111
```

```output2
16
16 15 14 13 12 11 10 9 8 7 6 5 4 3 2 1
```






```input3
101011010001100100011011001111011000011110010
```

```output3
16
13 6 1 7 12 5 4 15 14 16 10 11 3 8 9 2
```



