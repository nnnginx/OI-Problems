## 题目描述


The Merkle-Hellman Knapsack Cryptosystem was one of the earliest public key cryptosystems invented by Ralph Merkle and Martin Hellman in $1978$ . Here is its description

Alice chooses $n$ positive integers ${a_{1}, . . . , a_{n}}$ such that each $a_{i} > \sum^{i−1}_{j=1}a_{j},$ a positive integer $q$ which is greater than the sum of all $a_{i},$ and a positive integer $r$ which is coprime with $q$ . These $n + 2$ integers are Alice's private key.

Then Alice calculates $b_i = (a_{i} · r)$ mod $q$ . These $n$ integers are Alice's public key.

Knowing her public key, Bob can transmit a message of $n$ bits to Alice. To do that he calculates $s$ , the sum of $b_{i}$ with indices $i$ such that his message has bit $1$ in i-th position. This value $s$ is the encrypted message.

Note that an eavesdropper Eve, who knows the encrypted message and the public key, has to solve a (presumably hard) instance of the knapsack problem to find the original message. Meanwhile, after receiving $s$ , Alice can calculate the original message in linear time; we leave it to you as an exercise.

In this problem you deal with the implementation of the Merkle-Hellman Knapsack Cryptosystem in which Alice chose $q = 2^{64},$ for obvious performance reasons, and published this information. Since everyone knows her $q$ , she asks Bob to send her the calculated value $s$ taken modulo $2^{64}$ for simplicity of communication.

You are to break this implementation. Given the public key and an encrypted message, restore the original message.



## 输入格式


The first line contains one integer $n (1 \le n \le 64)$ .

Each of the next $n$ lines contains one integer $b_{i} (1 \le b_{i} < 2^{64}).$

The last line contains one integer $s$ mod $q$ -- the encrypted message $s$ taken modulo $q (0 \le s$ mod $q < 2^{64}).$

The given sequence $b_{i}$ is a valid public key in the described implementation, and the given value $s$ mod $q$ is a valid encrypted message.



## 输出格式


Output exactly $n$ bits ($0$ or $1$ digits) -- the original message.



## 题目大意
背包密码是一个简单的公钥密码系统，下面是它的具体过程：

- Alice 选择 $n$ 个正整数 $a_1,a_2,\cdots,a_n$，满足 $a_i> \sum\limits_{j=1}^{i-1} a_j$，再选择两个正整数 $q,r$，满足 $q> \sum\limits_{j=1}^n a_i$，$r,q$ 互质。这 $n + 2$ 个数是 Alice 的私钥。再计算 $b_i = (a_i\cdot r)\bmod q$，这 $n+2$ 个数是 Alice 的公钥。

- Bob 有一个 01 串 $t$，他知道 Alice 的公钥，$t$ 加密后得到 $s=\left(\sum\limits_{i=1}^n [t_i=1]b_i\right)\bmod q$. 他把这个 01 串加密后的结果发给了 Alice。那 Alice 就可以在线性时间内解出来。

你现在截获了 $s$，并知道 $b_i$ 和 $q$，其中 $q = 2^{64}$。请解出这个 01 串。

$n\le 64$，保证 $s,b_i$ 合法。

```input1
5
10
20
50
140
420
440

```

```output1
01001

```

## 提示
Time limit: 3 s, Memory limit: 512 MB. 



