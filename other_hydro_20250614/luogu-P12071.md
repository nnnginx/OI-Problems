## ��Ŀ����
������ [2014 ���廪��ѧ��Ϣѧ������](https://gitlink.org.cn/thusaa/thoi2014)��

## ��Ŀ����
Printed Circuit Board�����PCB����ӡˢ��·�壬�����Թ̶����ֵ���Ԫ������Ȼ����������������ʹ������ϵͳ�ܹ�ʵ����������Ҫ�Ĺ��ܡ���ˣ��������ӡ���һ���ܶ๤��ѧ���������ǵ��ӡ��Զ���ϵ��ͬѧ������Ҫ���յļ��ܡ�

�ִ���·�����ӡˢ�����Ƴɡ�ӡˢ��·�������ص���װ���Ԫ�����ա����ۣ������ʺ��ڹ����Ĵ��ģ��������ȻҲ�ʺϸ��ֵ���С������������·��Ļ����Ǿ��εģ��û������ֽ�ʰ��Ƴɡ��ڻ�����������ѹ��������һ��ܱ���ͭ������ӡˢ���ѵ�·ӡ��ͭ���ϣ����ø�ʴ���Ѳ���Ҫ��ͭ��ȥ�������µ�ͭ���㹹�ɵ�·���������С�ף�Ϳ����������������·����Ƴ��ˡ�

���ڼ��������ƣ���·����ͭ�ߵĿ����ȷ���ģ�����ͭ�߱���ƽ���ڵ�·��ı߽磨Ҳ����˵ͭ�߱���ƽ���������ᣩ��

![](https://cdn.luogu.com.cn/upload/image_hosting/c0efse5g.png)

������������ͼ���ǿ��еĵ�·�塣

���� R ͬѧ��Ҫ�����ܶ�ܶ��·�壬ÿ����·���������ɸ�����Ԫ��������Ҫ�����õ�·ʹ��ͭ�������е���Ԫ������ͨ���������ĵ�ͭ���١�

## �����ʽ
��һ���������������� $T,n$����ʾRͬѧ��Ҫ�����ĵ�·��������ÿ���·���ϵĵ���Ԫ������

�����������ݹ�ģ�Ӵ���˲����������Ӻ�������ɵķ�ʽ��

�ڶ������� $6$ �������� $a,c,Mx,My,seedx,seedy$���Լ�һ���ַ� $datatype$���������·�ʽ�������� $X_i,Y_i$��

$$X_0=seedx, X_i=((aX_{i-1}+c) \div 2^{16})\bmod 2^{16}$$

$$Y_0=seedy, Y_i=((aY_{i-1}+c) \div 2^{16})\bmod 2^{16}$$

�� $datatype$ Ϊ `B`����

$$(X_{in}\bmod Mx+Mx,Y_{in}\bmod My+My)$$
$$(X_{in+1}\bmod Mx+Mx,Y_{in+1}\bmod My+My)$$
$$(X_{in+2}\bmod Mx+Mx,Y_{in+2}\bmod My+My)$$
$$(X_{in+3}\bmod Mx+Mx,Y_{in+}\bmod My+My)$$
$$\dots$$
$$(X_{in+n-1}\bmod Mx_+Mx,Y_{in+n-1}\bmod My+My)$$

Ϊ�� $i (0 \le i \lt T)$ �������е� $n$ ������Ԫ�������ꡣ

�� $datatype$ Ϊ `B`����

$$(X_{in}\bmod Mx+Mx,Y_{in}\bmod My+My)$$
$$(X_{in+1}\bmod Mx+Mx,Y_{in+1}\bmod My+My)$$
$$(X_{in+2}\bmod Mx+Mx,Y_{in+2}\bmod My+My)$$
$$(X_{in+3}\bmod Mx,Y_{in+3}\bmod My)$$
$$\dots$$
$$(X_{in+n-1}\bmod Mx,Y_{in+n-1}\bmod My)$$

Ϊ�� $i (0 \le i \lt T)$ �������е� $n$ ������Ԫ�������ꡣ��**��ǰ������ĺ�������ֱ���� $Mx$ �� $My$**����

## �����ʽ
ÿ���������һ�У�������һ��������ʾ��̵�ͭ�߳��ȡ�

```input1
3 3
903527 47001 10 10 675 293 A
```

```output1
11
5
9
```

```input2
8 5
903527 47001 5 5 190 338 A
```

```output2
9
8
7
7
8
7
8
4
```

```input3
5 7
903527 47001 1000 1000 190 338 B
```

```output3
3364
3305
4076
3714
2969
```

## ��ʾ
**������ #1 ���͡�**

```
case0:(5,3) (6,0) (4,9) 
case1:(2,1) (1,4) (2,0) 
case2:(1,3) (0,7) (3,1)
```

![](https://cdn.luogu.com.cn/upload/image_hosting/8jkdlqid.png)

**������ #2 ���͡�**

```
case0: (0,3) (0,0) (1,1) (4,4) (0,1)
case1: (3,1) (2,3) (2,4) (4,3) (1,0)
case2: (3,2) (2,1) (0,2) (0,4) (3,1)
```

![](https://cdn.luogu.com.cn/upload/image_hosting/wj9yxar1.png)

**�����ݷ�Χ��**

���� $100\%$ �����ݣ�$n \le 7,T \le 10^6, a,c < 2^{31},Mx,My \le 2^{16}$��

���⹲ $20$ �����ݣ�ÿ�� $5$ �֡�

![](https://cdn.luogu.com.cn/upload/image_hosting/n3tts4tp.png)

**��С��ʿ��**

Ϊ�˷����ұ�д�����������ṩһ���������������ɵĴ��룬������Ҳο��������Դ�Ϊģ�壩��

## C/C++��

```cpp
int X[7000010],Y[7000010];
int n,T,a,c,Mx,My;
long long seedx,seedy;
char datatype[4];
//�������ݣ��������Mx��Myȡģ���ֵ������X,Y������������
void createList() {
int AD = (1 << 16) - 1;
  int i;
  for (i = 0;i < n*T;i++) {
    X[i] = seedx % Mx;
    Y[i] = seedy % My;
if (i % n < 3 && datatype[0] == 'B')
X[i] += Mx,Y[i] += My;
    seedx = (((a * seedx + c) >> 16) & AD);
    seedy = (((a * seedy + c) >> 16) & AD);
  }
}

int main() {
  scanf("%d%d%d%d%d%d%d%d%s",
&T, &n, &a, &c, &Mx, &My, &seedx, &seedy, datatype);
  createList();
//��ļ������
  return 0;
}
```

## Pascal��

```pas
var 
  ax,ay:array[0..7000000] of longint;
  n,T,a,c,Mx,My:longint;
  seedx,seedy:int64;
  datatype:char;
  i,j:longint;
//�������ݣ��������Mx��Myȡģ���ֵ������ax,ay������������
procedure createList;
var AD,i:longint;
begin
  AD := (1 shl 16) - 1;
  for i:=0 to n * T - 1 do
  begin
    ax[i] := seedx mod Mx;
    ay[i] := seedy mod My;
    if ((i mod n < 3) and (datatype = 'B')) then
    begin
      ax[i] := ax[i] + Mx;
      ay[i] := ay[i] + My;
    end;
    seedx := (((a * seedx + c) shr 16) and AD);
    seedy := (((a * seedy + c) shr 16) and AD);
  end;
end;
begin
  read(T,n,a,c,Mx,My,seedx,seedy);
  read(datatype);
  while (datatype = ' ') do read(datatype);
  createList;
  //��ļ������
end.
```

