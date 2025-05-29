## ��Ŀ����

�����˶�ã�Crash ��Ҫӭ������˼ĺ�����١�������������ƻ��ŵ����������Ρ��ڻ������� $n$ �����ξ��㣬Crash �� $1$ �� $n$ �� $n$ ������������Щ�����š����ξ���֮��ͨ��˫���·������

���ڻ��ǵĻ����͵����кܴ�Ĳ��죬������·�ĳɱ�Ҳ��Խϸߡ�Ϊ�˽�Լ�ɱ���ֻ�� $n-1$ ����·��������Щ���ξ��㣬�������Ա�֤�κ�������ͬ�����ξ��㶼ͨ��·��������Crash Ԥ���ڻ������ϲ�������Щ�������Ϣ���������ϵĽ��ܣ�����ÿ�����㶼��һ��ӡ��ֵ�����ӡ��ֵΪһ������������������У�����ѡ��һ��������Ϊ���еĿ�ʼ�������Ŵ��ڵĵ�·���������������档Ϊ��ʹ���в��Ե÷�ζ��Crash ���ᾭ��ͬһ�����㳬��һ�Ρ�

Crash ����������ж�����һ������ָ����Ҳ���������������о����ӡ��ֵ֮�͡����� Crash �Ǹ���ֵ�С���ѣ������ھ����ӡ��ֵ�ᷢ���ı䣬������Ҳû�о�����Ӧ�ô��ĸ����㿪ʼ���С������ϣ������дһ������������һ���򵥵����񣺸��ݵ�ǰ����ÿ�������ӡ��ֵ�������ĳ�����㿪ʼ�������ܻ�õ����Ŀ���ָ����

## �����ʽ

����ĵ�һ�а���һ���ַ���һ�������� $n$���ַ�Ϊ `A`��`B`��`C` �е�һ����������ʾ����������ݵ����ͣ������������ݹ�ģ��Լ������

�ڶ��а��� $n$ ���ÿո�������������� $i$ ��������ʾ Crash �� $i$ �ž���ĳ�ʼӡ��ֵ��

������ $n-1$ �У�ÿ������������ $a,b$����ʾ�� $a$ �ž��㵽 $b$ �ž�����һ�������·������

�����һЩָ�ָ��ֻ�����������ָ�ʽ��

1. `Change u x` �� $u$ �ž����ӡ��ֵ�޸�Ϊ $x$��
2. `Query u` ѯ�ʴ� $u$ �ž��㿪ʼ�ܻ�õ����Ŀ���ָ����
3. `Done` �յ����ָ�����ĳ���Ӧ�ý�����

## �����ʽ

����ÿ�� `Query` ָ������Ӧ��������ָ����

## ��������#1

```plain
A 6
6 5 -4 3 -2 1
1 2
1 3
1 4
3 5
3 6
Query 3
Query 4
Change 6 10
Query 3
Change 2 -5
Query 3
Query 4
Done
```

## ������� #1

```plain
7
14
7
6
15
```

## �������� #2

```plain
B 5
5 -4 3 -2 1
1 2
2 3
3 4
4 5
Query 3
Change 5 10
Query 3
Query 2
Change 2 2
Query 3
Done
```

## ������� #2

```plain
4
11
7
11
```

## ���ݹ�ģ��Լ��

�������ݷ�Ϊ `A`��`B`��`C` ���࣬�������еĲ������ݶ����㣺���κ�ʱ��һ������ӡ��ֵ�ľ���ֵ������ $10^4$����������ĵ�·һ����������Ŀ������Ҫ�󣬼�ʹ������������ͬ�ľ��㶼��ͨ��·��������

���� `A` �����ݣ�ռ $20\%$ �ķ��������㣺$n$ ��ָ��������������� $10^3$��

���� `B` �����ݣ�ռ $40\%$ �ķ��������㣺$n$ ��ָ��������������� $10^5$��������ĵ� $i$ ����·�������� $i$ �ž���� $i+1$ �ž��㣨������� 2����

���� `C` �����ݣ�ռ $40\%$ �ķ��������㣺$n$ ��ָ��������������� $10^5$�����κ�һ�����㵽 $1$ �ž�����Ҫͨ���ĵ�·���������� $40$��

�������е� $a,b,u$������ $1\leq a,b,u\leq n$��

**���ر�˵����** �������ݴ�С����Ϊ 5MB����ֻ�öԲ���ʱ�������ļ�����ѹ����������ĺ������Խ�ѹ���������ļ�ת��Ϊԭʼ�����ļ����������� `infile` �ж���ѹ���������ļ�������ѹ����������ļ������ `outfile` �У�

C/C++ �汾��

```cpp
void Uncompress(FILE *infile, FILE *outfile) {
  int N, M, L, now, A, B, Q, tmp, i;
  char type = getc(infile);
  fscanf(infile, "%d%d%d", &N, &M, &L);
  fscanf(infile, "%d%d%d%d", &now, &A, &B, &Q);
  fprintf(outfile, "%c %d\n", type, N);
  for (i = 1; i <= N; i ++) {
    now = (now * A + B) % Q, tmp = now % 10000;
    now = (now * A + B) % Q; 
    if (now * 2 < Q) tmp *= -1;
    if (i < N) fprintf(outfile, "%d ", tmp);
    else fprintf(outfile, "%d\n", tmp);
  }
  for (i = 1; i < N; i ++) {
    now = (now * A + B) % Q;
    tmp = (i < L) ? i : L;
    fprintf(outfile, "%d %d\n", i - now % tmp, i + 1);
  }
  for (i = 1; i < M; i ++) {
    now = (now * A + B) % Q;
    if (now * 3 < Q) {
      now = (now * A + B) % Q;
      fprintf(outfile, "Query %d\n", now % N + 1);
    }
    else {
      now = (now * A + B) % Q, tmp = now % 10000;
      now = (now * A + B) % Q;
      if (now * 2 < Q) tmp *= -1;
      now = (now * A + B) % Q;
      fprintf(outfile, "Change %d %d\n", now % N + 1, tmp);
    }
  }
  fprintf(outfile, "Done\n");
}
```

Pascal �汾��

```pascal
procedure Uncompress(var infile, outfile : text);
  var N, M, L, now, A, B, Q, tmp, i : longint;
  ch : char;
  begin read(infile, ch, N, M, L, now, A, B, Q);
  writeln(outfile, ch, ' ', N);
  for i := 1 to N do begin
    now := (now * A + B) mod Q;
    tmp := now mod 10000;
    now := (now * A + B) mod Q;
    if now * 2 < Q then tmp := -tmp;
    if i < n then write(outfile, tmp, ' ')
    else writeln(outfile, tmp);
  end;
  for i := 1 to N - 1 do begin
    now := (now * A + B) mod Q;
    if i < L then tmp := i
    else tmp := L;
    writeln(outfile, i - now mod tmp, ' ', i + 1);
  end;
  for i := 1 to M - 1 do begin
    now := (now * A + B) mod Q;
    if now * 3 < Q then begin
      now := (now * A + B) mod Q;
      writeln(outfile, 'Query ', now mod N + 1);
    end
    else begin
      now := (now * A + B) mod Q;
      tmp := now mod 10000;
      now := (now * A + B) mod Q;
      if now * 2 < Q then tmp := -tmp;
      now := (now * A + B) mod Q;
      writeln(outfile, 'Change ', now mod N + 1, ' ', tmp);
    end;
  end;
  writeln(outfile, 'Done');
end;
```

�������һ����������ӡ�`travel_compressed.in` ��ʾѹ���������ļ��� `travel.in` ��ʾ��ѹ����������ļ���

`travel_compressed.in`

```plain
A 5 7 3 17627 543 14278 380043
```

`travel.in`

```plain
A 5
-4664 7653 -3584 -210 5852
1 2
1 3
2 4
3 5
Change 5 -3724
Query 4
Change 3 -5628
Query 2
Change 5 569
Query 5
Done
```

