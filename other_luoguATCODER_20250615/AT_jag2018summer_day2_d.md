# AT_jag2018summer_day2_d Knapsack And Queries

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jag2018summer-day2/tasks/jag2018summer_day2_d

First, you are given a positive integer $ MOD $.

You have a knapsack, this is empty at first.

You have to perform $ Q $ queries.

- In each query, you have first to perform either `ADD` or `REMOVE` operation, and then perform `FIND` operation.
- `ADD` operation : You are given positive integers $ w,\ v $. You put the cookie whose weight is $ w $ and whose value is $ v $ to the knapsack.
- `REMOVE` operation : You take out the cookie with the smallest weight from the knapsack and eat it.
- `FIND` operation : You are given non-negative integers $ l,\ r $. You answer the following question:
  
  
  - Can you choose cookies from the knapsack so that the sum $ X $ of the weights of selected cookies satisfies $ l\ \leq\ (X\ {\rm\ mod}\ MOD)\ \leq\ r $
  - If you can't, output `-1`.
  - Otherwise, output the maximum sum of the values of selected cookies.

## 输入格式

Input is given from Standard Input in the following format:

> $ MOD $ $ Q $ $ t'_1 $ $ w'_1 $ $ v'_1 $ $ l'_1 $ $ r'_1 $ $ t'_2 $ $ w'_2 $ $ v'_2 $ $ l'_2 $ $ r'_2 $ : $ t'_Q $ $ w'_Q $ $ v'_Q $ $ l'_Q $ $ r'_Q $

- $ 0\ \leq\ t'_i,\ w'_i,\ v'_i,\ l'_i,\ r'_1\ \leq\ 2^{30}\ -\ 1 $
- Queries are **Online Query**. You can get $ t_i,\ w_i,\ v_i,\ l_i,\ r_i $ by decoding $ t'_i,\ w'_i,\ v'_i,\ l'_i,\ r'_i $.
- $ t_i $ is query type.
  
  
  - When $ t_i\ =\ 1 $, it involves `ADD` operation + `FIND` operation.
  - When $ t_i\ =\ 2 $, it involves `REMOVE` operation + `FIND` operation.
- When $ t_i\ =\ 2 $, you can assume that $ w_i=0 $ and $ v_i\ =\ 0 $.

## 输出格式

Print results of `FIND` operation, one per line.

## 输入输出样例 #1

### 输入 #1

```
10
7
281614559 249378726 433981056 466775634 683612866
727071329 787572584 591471796 328464426 757737734
279580343 240336097 538846427 808491898 224313807
222498984 42804452 371605808 667115067 791865961
68683864 1045549765 515479514 1067782238 349547144
907343711 381772625 149003422 879314974 953881571
883899098 700164610 414212891 752949213 972845634
```

### 输出 #1

```
10
0
-1
21
-1
11
111
```

## 输入输出样例 #2

### 输入 #2

```
7
20
281614559 249378726 433981094 466775639 683612870
59536386 999828879 241246766 434670565 174365647
172060134 848462699 857413429 182122460 807914643
808426426 600772095 829463884 974102196 354283529
370037909 1024921880 664216868 194331103 140834169
917331875 242953442 205247688 335469789 1055568137
823475244 641321246 617915164 160300810 1073617378
892669150 939175632 904628449 606339993 1059849410
829170894 436718235 288920513 228195002 55212938
772189413 373108543 94133155 610930061 513937768
986619331 175674265 812546186 865335970 605634588
880196843 1071068047 723408215 587598264 380801783
393196081 141080294 584230885 135343295 661927186
5740819 967233824 22597607 888639499 467454437
365679801 515258603 989059385 962028117 761163096
357270919 737051059 569528959 935653628 70506031
869282414 947492121 280522456 96822010 856514221
155948699 826430734 291243254 381421299 617876780
980891674 833928389 1048677341 522527723 223764850
50617939 963598173 281959650 499436870 47455938
```

### 输出 #2

```
0
134
90
158
-1
22
238
269
179
189
121
53
41
41
-1
58
-1
84
-1
149
```

## 说明/提示

### Constraints

- $ 2\ \leq\ MOD\ \leq\ 500 $
- $ 1\ \leq\ Q\ \leq\ 100,000 $
- $ 1\ \leq\ w_i,\ v_i\ \leq\ 10^9 $
- $ 0\ \leq\ l_i\ \leq\ r_i\ \leq\ MOD-1 $
- The cookie given by an `ADD` operation is strictly heavier than any cookie which was added by a previous `ADD` operation.
- When executing `REMOVE` operation, the knapsack isn't empty.
- Queries are **Online Query**. Queries are encrypted as described later.

### Decryption

We prepare the decryption code with C++11 (or later), Java, D, C#.

Use `class Crypto` for decryption, the code of `class Crypto` is below.

C++

 ```
#include <cstdint> //uint8_t, uint32_t

class Crypto {
public:    
    Crypto() {
        sm = cnt = 0;
        seed();
    }

    int decode(int z) {
        z ^= next();
        z ^= (next() << 8);
        z ^= (next() << 16);
        z ^= (next() << 22);
        return z;
    }

    void query(long long z) {
        const long long B = 425481007;
        const long long MD = 1000000007;
        cnt++;
        sm = ((sm * B % MD + z) % MD + MD) % MD;
        seed();
    }
private: 
    long long sm;
    int cnt;

    uint8_t data[256];
    int I, J;

    void swap_data(int i, int j) {
        uint8_t tmp = data[i];
        data[i] = data[j];
        data[j] = tmp;    
    }

    void seed() {
        uint8_t key[8];
        for (int i = 0; i < 4; i++) {
            key[i] = (sm >> (i * 8));
        }
        for (int i = 0; i < 4; i++) {
            key[i+4] = (cnt >> (i * 8));
        }

        for (int i = 0; i < 256; i++) {
            data[i] = i;
        }
        I = J = 0;

        int j = 0;
        for (int i = 0; i < 256; i++) {
            j = (j + data[i] + key[i%8]) % 256;
            swap_data(i, j);
        }
    }

    uint8_t next() {
        I = (I+1) % 256;
        J = (J + data[I]) % 256;
        swap_data(I, J);
        return data[(data[I] + data[J]) % 256];
    }
};
```

Java

 ```
public class Main {
    public static class Crypto {
        public Crypto() {
            sm = cnt = 0;
            seed();
        }
        public int decode(int z) {
            z ^= next();
            z ^= (next() << 8);
            z ^= (next() << 16);
            z ^= (next() << 22);
            return z;
        }
        public void query(long z) {
            final long B = 425481007;
            final long MD = 1000000007;
            cnt++;
            sm = ((sm * B % MD + z) % MD + MD) % MD;
            seed();
        }

        long sm;
        int cnt;

        byte data[] = new byte[256];
        int I, J;

        int asUint(byte x) {
            int y = x;
            return y & 0xff;
        }
        void seed() {
            byte key[] = new byte[8];
            for (int i = 0; i < 4; i++) {
                key[i] = (byte)(sm >>> (i * 8));
            }
            for (int i = 0; i < 4; i++) {
                key[i+4] = (byte)(cnt >>> (i * 8));
            }

            for (int i = 0; i < 256; i++) {
                data[i] = (byte)i;
            }
            I = J = 0;

            int j = 0;
            for (int i = 0; i < 256; i++) {
                j = (j + asUint(data[i]) + asUint(key[i % 8])) % 256;
                byte tmp = data[i];
                data[i] = data[j];
                data[j] = tmp;
            }
        }
        int next() {
            I = (I+1) % 256;
            J = (J+asUint(data[I])) % 256;
            byte tmp = data[I];
            data[I] = data[J];
            data[J] = tmp;
            return asUint(data[(asUint(data[I]) + asUint(data[J])) % 256]);
        }
    }
    public static void main(String[] args) {
        ...
    }
}
```

D

 ```
class Crypto {
public:
    this() {
        sm = cnt = 0;
        seed();
    }

    int decode(int z) {
        z ^= next();
        z ^= (next() << 8);
        z ^= (next() << 16);
        z ^= (next() << 22);
        return z;
    }

    void query(long z) {
        immutable static long B = 425481007;
        immutable static long MD = (10^^9)+7;
        cnt++;
        sm = ((sm * B % MD + z) % MD + MD) % MD;
        seed();
    }
private:
    import std.algorithm : swap;
    long sm;
    int cnt;

    ubyte[256] data;
    int I, J;
    void seed() {
        ubyte[8] key;
        foreach (i; 0..4) {
            key[i] = cast(ubyte)(sm >> (i*8));
        }
        foreach (i; 0..4) {
            key[i+4] = cast(ubyte)(cnt >> (i*8));
        }

        foreach (i; 0..256) {
            data[i] = cast(ubyte)(i);
        }
        I = J = 0;

        int j = 0;
        foreach (int i; 0..256) {
            j = (j + data[i] + key[i%8]) % 256;
            swap(data[i], data[j]);
        }        
    }

    ubyte next() {
        I = (I+1) % 256;
        J = (J + data[I]) % 256;
        swap(data[I], data[J]);
        return data[(data[I] + data[J]) % 256];
    }
}
```

C#

 ```
class Crypto {
    public Crypto() {
        sm = cnt = 0;
        data = new byte[256];
        seed();
    }

    public int decode(int z) {
        z ^= next();
        z ^= (next() << 8);
        z ^= (next() << 16);
        z ^= (next() << 22);
        return z;
    }

    public void query(long z) {
        const long B = 425481007;
        const long MD = 1000000007;
        cnt++;
        sm = ((sm * B % MD + z) % MD + MD) % MD;
        seed();
    }

    long sm;
    int cnt;

    byte[] data;
    int I, J;

    void seed() {
        byte[] key = new byte[8];
        for (int i = 0; i < 4; i++) {
            key[i] = (byte)(sm >> (i*8));
        }
        for (int i = 0; i < 4; i++) {
            key[i+4] = (byte)(cnt >> (i*8));
        }

        for (int i = 0; i < 256; i++) {
            data[i] = (byte)i;
        }
        I = J = 0;

        int j = 0;
        for (int i = 0; i < 256; i++) {
            j = (j + data[i] + key[i%8]) % 256;
            byte tmp = data[i];
            data[i] = data[j];
            data[j] = tmp;
        }
    }

    byte next() {
        I = (I+1) % 256;
        J = (J + data[I]) % 256;
        byte tmp = data[I];
        data[I] = data[J];
        data[J] = tmp;
        return data[(data[I] + data[J]) % 256];
    }
}
```

The procedure of decrypto:

- First, you make an instance of `class Crypto`.
- In each query,
  - call the `decode` function for each of $ t',\ w',\ v',\ l',\ r' $ in order. The return values are $ t,\ w,\ v,\ l,\ r $.
  - call the `query` function with the result of the `FIND` operation.

The sample code of C++ is below.

 ```
#include <cstdio>
#include <cstdlib>
#include <cstdint> //uint8_t, uint32_t

class Crypto {
    ...
};

int main() {
    int MOD, Q;
    scanf("%d %d", &MOD, &Q);
    Crypto c;
    for (int i = 0; i < Q; i++) {
        int t, w, v, l, r;
        scanf("%d %d %d %d %d", &t, &w, &v, &l, &r);
        t = c.decode(t);
        w = c.decode(w);
        v = c.decode(v);
        l = c.decode(l);
        r = c.decode(r);
        if (t == 1) {
            (add candy(w, v))
        } else {
            (delete candy)
        }
        long long ans = (answer for query(l, r));
        c.query(ans);
        printf("%lld\n", ans);
    }
}
```

The sample codes of Java, D, C# are below.

Java

 ```
import java.io.PrintWriter;
import java.util.Scanner;

public class Main {
    public static class Crypto {
        ...
    }    
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in); //!!warning!! : Java's scanner is slow
        PrintWriter out = new PrintWriter(System.out);
        int MOD = in.nextInt();
        int Q = in.nextInt();

        Crypto c = new Crypto();
        for (int i = 0; i < Q; i++) {
            int t, w, v, l, r;
            t = c.decode(in.nextInt());
            w = c.decode(in.nextInt());
            v = c.decode(in.nextInt());
            l = c.decode(in.nextInt());
            r = c.decode(in.nextInt());
            if (t == 1) {
                (add candy(w, v))
            } else {
                (delete candy)
            }
            long ans = (answer for query(l, r));
            c.query(ans);
            out.println(ans);
        }
        out.flush();
    }
}
```

D

 ```
class Crypto {
    ...
}
int main() {
    import std.stdio;
    int MOD, Q;
    readf("%d\n%d\n", &MOD, &Q);
    Crypto c = new Crypto();
    foreach (i; 0..Q) {
        int t, w, v, l, r;
        readf("%d %d %d %d %d\n", &t, &w, &v, &l, &r);
        t = c.decode(t);
        w = c.decode(w);
        v = c.decode(v);
        l = c.decode(l);
        r = c.decode(r);
        if (t == 1) {
            (add candy(w, v))
        } else {
            (delete candy)
        }
        long ans = (answer for query(l, r));
        c.query(ans);
        writeln(ans);
    }
    return 0;
}
```

C#

 ```
using System;
using System.IO;

class Crypto {
    ...
}
class Myon {
    static void Main() {
        var writer = new StreamWriter(Console.OpenStandardOutput()){AutoFlush = false}; //fast writer
        Console.SetOut(writer);

        int MOD = int.Parse(Console.ReadLine());
        int Q = int.Parse(Console.ReadLine());
        Crypto c = new Crypto();
        for (int i = 0; i < Q; i++) {
            var inputs = Console.ReadLine().Split(' ');
            int t, w, v, l, r;
            t = c.decode(int.Parse(inputs[0]));
            w = c.decode(int.Parse(inputs[1]));
            v = c.decode(int.Parse(inputs[2]));
            l = c.decode(int.Parse(inputs[3]));
            r = c.decode(int.Parse(inputs[4]));
            if (t == 1) {
                (add candy(w, v))
            } else {
                (delete candy)
            }
            long ans = (answer for query(l, r));
            c.query(ans);
            Console.WriteLine(ans);
        }
        Console.Out.Flush();
    }
}
```

Remark:

- You don't need to find vulnerability of this encryption.
- `class Crypto` consume time at most about $ 200 $ ms when $ Q\ =\ 100,000 $.

### Sample Explanation 1

The result of decoding this input is as follows. ``` 10 7 1 5 10 5 5 2 0 0 0 9 1 7 10 2 4 1 12 11 9 9 2 0 0 1 1 1 22 10 2 3 1 32 100 4 4 ``` Knapsack Selected Cookies (w, v) = {(5, 10)} {(5, 10)} {} {} {(7, 10)} -1 {(7, 10), (12, 11)} {(7, 10), (12, 11)} {(12, 11)} -1 {(12, 11), (22, 10)} {(12, 11)} {(12, 11), (22, 10), (32, 100)} {(12, 11), (32, 100)}

### Sample Explanation 2

The result of decoding this input is as follows. ``` 7 20 1 5 44 0 1 1 11 90 0 3 2 0 0 3 4 1 18 68 1 6 1 25 32 2 3 1 31 22 2 3 1 32 26 1 5 1 36 31 3 6 2 0 0 2 5 1 43 10 3 6 2 0 0 5 6 2 0 0 3 4 2 0 0 2 4 2 0 0 1 5 2 0 0 3 5 1 49 48 0 4 2 0 0 1 5 1 50 36 0 6 1 56 48 3 5 1 59 17 3 5 ```