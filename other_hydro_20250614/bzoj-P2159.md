## ��Ŀ����

Crash С�������������һ����Ϸ�������� 5��Civilization V�����������Ϸ�У���ҿ��Խ����ͷ�չ�Լ��Ĺ��ң�ͨ���⽻�ͱ�Ĺ��ҽ���������ͨ��ս��������Ĺ��ҡ�

���� Crash �Ѿ�ӵ����һ�� $n$ �����еĹ��ң���Щ����֮��ͨ����·���������ڽ����·���л��ѵģ���� Crash ֻ�޽��� $n-1$ ����·������Щ���У��������Ա�֤�����������ж���·����ͨ��

����Ϸ�У�Crash ��Ҫѡ��һ��������Ϊ���Ĺ��ҵ��׶���ѡ���׶���Ҫ���Ǻܶ�ָ�꣬��һ��ָ���������ģ�

$$
S(i)=\sum_{j=1}^n \operatorname{dist}(i,j)^k
$$

���� $S(i)$ ��ʾ�� $i$ �����е�ָ��ֵ��$\operatorname{dist}(i, j)$ ��ʾ�� $i$ �����е��� $j$ ��������Ҫ�����ĵ�·��������Сֵ��$k$ Ϊһ��������Ϊ��������

��� Crash ������һ���򵥵����񣺸�������֮��ĵ�·������ÿ�����У����������е�ָ��ֵ������ָ��ֵ���ܻ�ܴ�������ֻ��Ҫ�������� $\bmod\; 10007$ ��ֵ��

## �����ʽ

����ĵ�һ�а������������� $n$ �� $k$��

������ $n-1$ �У�ÿ������������ $u,v (1 \leq u, v \leq n)$����ʾ�� $u$ �����к͵� $v$ ������֮���е�·�ࡣ��Щ��·��֤�ܷ�����Ŀ��Ҫ��

## �����ʽ

����� $n$ �У�ÿ��һ������������ $i$ �е���������ʾ�� $i$ �����е�ָ��ֵ $\bmod\; 10007$ ��ֵ��

## ��������

```plain
5 2
1 2
1 3
2 4
2 5
```

## �������

```plain
10
7
23
18
18
```

## ���ݹ�ģ��Լ��

$20\%$ ���������� $n \leq 5\times 10^3$��$k \leq 30$��

$50\%$ ���������� $n \leq 5\times 10^4$��$k \leq 30$��

$100\%$ ���������� $n \leq 5\times 10^4$��$k \leq 150$��

**���ر�ע�⡿** �������ݴ�С����Ϊ 5MB����ֻ�öԲ���ʱ�������ļ�����ѹ����������ĺ������Խ�ѹ���������ļ�ת��Ϊԭʼ�����ļ����������� `infile` �ж���ѹ���������ļ�������ѹ����������ļ������ `outfile` �У�

C/C++ �汾��

```cpp
void Uncompress(FILE *infile, FILE *outfile) {
  int N, k, L, i, now, A, B, Q, tmp;
  fscanf(infile, "%d%d%d", &N, &k, &L);
  fscanf(infile, "%d%d%d%d", &now, &A, &B, &Q);
  fprintf(outfile, "%d %d\n", N, k);
  for (i = 1; i < N; i ++) {
    now = (now * A + B) % Q;
	tmp = (i < L) ? i : L;
	fprintf(outfile, "%d %d\n", i - now % tmp, i + 1);
  }
}
```

Pascal �汾��

```pascal
procedure Uncompress(var infile, outfile : text);
var N, k, L, i, now, A, B, Q, tmp : longint; begin
  read(infile, N, k, L, now, A, B, Q);
  writeln(outfile, N, ' ', k);
  for i := 1 to N - 1 do begin
	now := (now * A + B) mod Q;
	if i < L then tmp := i
	else tmp := L;
	writeln(outfile, i - now mod tmp, ' ', i + 1);
  end;
end;
```

�������һ����������ӡ�`civiliazation_compressed.in`��ʾѹ���������ļ��� `civilization.in`��ʾ��ѹ����������ļ���

`civilization_compressed.in`

```plain
7 26 4 29643 2347 5431 54209
```

`civilization.in`

```plain
7 26
1 2
2 3
2 4
3 5
4 6
5 7
```

2016.2.19 ����ʱ��Ϊ 10s

