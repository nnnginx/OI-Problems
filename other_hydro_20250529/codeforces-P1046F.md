## Description

<div><p>After finding and moving to the new planet that supports human life, discussions started on which currency should be used. After long negotiations, Bitcoin was ultimately chosen as the universal currency.</p><p>These were the great news for Alice, whose grandfather got into Bitcoin mining in 2013, and accumulated a lot of them throughout the years. Unfortunately, when paying something in bitcoin everyone can see how many bitcoins you have in your public address wallet. </p><p>This worried Alice, so she decided to split her bitcoins among multiple different addresses, so that every address has at most $x$ satoshi (1 bitcoin = $10^8$ satoshi). She can create new public address wallets for free and is willing to pay $f$ fee in satoshi per transaction to ensure acceptable speed of transfer. The fee is deducted from the address the transaction was sent from. Tell Alice how much total fee in satoshi she will need to pay to achieve her goal.</p></div><div class="input-specification"><p>First line contains number $N$ ($1 \leq N \leq 200\,000$) representing total number of public addresses Alice has.</p><p>Next line contains $N$ integer numbers $a_i$ ($1 \leq a_i \leq 10^9$) separated by a single space, representing how many satoshi Alice has in her public addresses.</p><p>Last line contains two numbers $x$, $f$ ($1 \leq f &lt; x \leq 10^9$) representing maximum number of satoshies Alice can have in one address, as well as fee in satoshies she is willing to pay per transaction. </p></div><div class="output-specification"><p>Output one integer number representing total fee in satoshi Alice will need to pay to achieve her goal.</p></div>

## Input

<p>First line contains number $N$ ($1 \leq N \leq 200\,000$) representing total number of public addresses Alice has.</p><p>Next line contains $N$ integer numbers $a_i$ ($1 \leq a_i \leq 10^9$) separated by a single space, representing how many satoshi Alice has in her public addresses.</p><p>Last line contains two numbers $x$, $f$ ($1 \leq f &lt; x \leq 10^9$) representing maximum number of satoshies Alice can have in one address, as well as fee in satoshies she is willing to pay per transaction. </p>

## Output

<p>Output one integer number representing total fee in satoshi Alice will need to pay to achieve her goal.</p>

## Samples

```input1
3
13 7 6
6 2

```

```output1
4

```




## Note

<p>Alice can make two transactions in a following way:</p><p>0. 13 7 6 (initial state)</p><p>1. 6 7 6 5 (create new address and transfer from first public address 5 satoshies)</p><p>2. 6 4 6 5 1 (create new address and transfer from second address 1 satoshi)</p><p>Since cost per transaction is 2 satoshies, total fee is 4.</p>
