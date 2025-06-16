## ��Ŀ����
> �����ϣ��������Ǹ�ά�ġ�

## ��Ŀ����
Cirno ������һֻ $n$ ά���ϣ������ $S(0,0,...,0)$ ���� $T(1,1,...,1)$ ��

���������� $1\times1\times...\times1$ �ķ����У�����ÿһ��ֻ������һ���������ڵĵ㡣

���� Cirno �뿼��������������ҵ��������� $S$ �� $T$ ��·������û�н���( �� $S$, $T$ )��

��Ҫ���㹹������һ��·����

## �����ʽ
һ�У�һ������ $n$ ��

## �����ʽ
��һ�У�һ������ $t$����ʾ����·������

���� $t$ �У�ÿ��һ���Ϸ�·����

�Ϸ�·����ʾ��ʽ :

> $S$ [�ո�] $P_1$ [�ո�] $P_2$ [�ո�] ... [�ո�] $T$

���� $P_i$ ��һ��������ѹ���� $01$ �� ��ʾһ�� $n$ ά���ꡣ

**�벻Ҫ�������Ŀո�**��

```input1
2
```

```output1
2
0 1 3
0 2 3
```

## ��ʾ
**������ʹ�� Special Judge��**

### Sample1����

�� $1$ ��·����$(0,0) \rightarrow (0,1) \rightarrow (1,1)$

�� $2$ ��·����$(0,0) \rightarrow (1,0) \rightarrow (1,1)$

���߳��� $S$ �� $T$ �޽��㡣

### ���ݷ�ΧԼ��

**�����ⲻ����������ԣ��������ݶȡ�**

���� 100% ������ $3 \le n \le 60$��

### ���ô���Ƭ��

 - ������ѹλ����

```cpp
/**
 * For only cpp11, cpp14, cpp17, cpp20.
 *
 * @param: __s : The binary high-dimension position inputed.
 * @return: Standard output format( U64 ).
**/

unsigned long long zip( std::string __s ) 
  { unsigned long long __r = 0;
    for( auto __c : __s ) 
      { ( __r <<= 1ull ) |= ( __c - 0x30 ); }
    return __r; }

```
 - SPJ����
```cpp
//SPJ
#include "testlib.h"
#include<bits/stdc++.h>

typedef unsigned long long ULL;
typedef std::vector<std::string> SEQ;
typedef std::string STR;

SEQ split( std::string _par, char _sgn )
  { SEQ _rat = SEQ();
	STR _rem = STR();
	
    for( char __c : _par )
      { if( __c = _sgn ) _rat.push_back( _rem ), _rem = "";
	    else _rem += __c; }
	
	if( _rem != "" ) _rat.push_back( _rem );
	
	return _rat; }

ULL to_ULL( std::string _str ) 
  { ULL _rat = 0;
	
	for( char __c : _str )
	  { ( _rat *= 10ull ) += (ULL)( __c - '0' ); }
	
	return _rat; }

bool isPw2( ULL x )
  { return !( x & (x - 1ull) ); }

std::map<ULL, bool> MP;

int main(int argc, char* argv[]) {
    registerTestlibCmd(argc, argv);
	
	ULL n = inf.readLong();
	ULL S = 0, T = (1ull << n) - 1ull;
	ULL N = ouf.readLong();
	
	if( N != n ) quitf( _wa, "Count paths wrongly." );
	
	ouf.readEoln();
	
    while( n -- ) {
    	std::string path = ouf.readLine();
    
    	ULL _lst = 0;
    	
    	for( auto N : split( path, " " ) )
    	  { ULL _now = to_ULL( N );
    		if( _now != S and _now != T and MP[_now] ) 
			  { quitf( _wa, "Paths crossing" ); }
    	    if( !isPw2( _now ^ _lst ) ) 
			  { quitf( _wa, "Wrong path format" ); }
    	    _lst = _now; MP[_now] = true; }
    	
    	if( _lst != T ) quitf( _wa, "Wrong path ending" );
	}
	
	quitf( _ok, "Accepted" );
	
    return 0;
} 
```


