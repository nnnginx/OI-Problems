## Description

<div><p>A Large Software Company develops its own social network. Analysts have found that during the holidays, major sporting events and other significant events users begin to enter the network more frequently, resulting in great load increase on the infrastructure.</p><p>As part of this task, we assume that the social network is <span class="tex-span">4<i>n</i></span> processes running on the <span class="tex-span"><i>n</i></span> servers. All servers are absolutely identical machines, each of which has a volume of RAM of <span class="tex-span">1</span> GB = <span class="tex-span">1024</span> MB <span class="tex-span"><sup class="upper-index">(1)</sup></span>. Each process takes 100 MB of RAM on the server. At the same time, the needs of maintaining the viability of the server takes about <span class="tex-span">100</span> more megabytes of RAM. Thus, each server may have up to <span class="tex-span">9</span> different processes of social network.</p><p>Now each of the <span class="tex-span"><i>n</i></span> servers is running exactly <span class="tex-span">4</span> processes. However, at the moment of peak load it is sometimes necessary to replicate the existing <span class="tex-span">4<i>n</i></span> processes by creating <span class="tex-span">8<i>n</i></span> new processes instead of the old ones. More formally, there is a set of replication rules, the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ 4<i>n</i></span>) of which has the form of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> → (<i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>)</span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) are the numbers of servers. This means that instead of an old process running on server <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, there should appear two new copies of the process running on servers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>. The two new replicated processes can be on the same server (i.e., <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> may be equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>) or even on the same server where the original process was (i.e. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> may be equal to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> or <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>). During the implementation of the rule <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> → (<i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>)</span> first the process from the server <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is destroyed, then appears a process on the server <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, then appears a process on the server <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>There is a set of <span class="tex-span">4<i>n</i></span> rules, destroying all the original <span class="tex-span">4<i>n</i></span> processes from <span class="tex-span"><i>n</i></span> servers, and creating after their application <span class="tex-span">8<i>n</i></span> replicated processes, besides, on each of the <span class="tex-span"><i>n</i></span> servers will be exactly <span class="tex-span">8</span> processes. However, the rules can only be applied consecutively, and therefore the amount of RAM of the servers imposes limitations on the procedure for the application of the rules.</p><p>According to this set of rules determine the order in which you want to apply all the <span class="tex-span">4<i>n</i></span> rules so that at any given time the memory of each of the servers contained at most <span class="tex-span">9</span> processes (old and new together), or tell that it is impossible.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30 000</span>) — the number of servers of the social network.</p><p>Next <span class="tex-span">4<i>n</i></span> lines contain the rules of replicating processes, the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ 4<i>n</i></span>) of these lines as form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and describes rule <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> → (<i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>It is guaranteed that each number of a server from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs four times in the set of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and eight times among a set that unites all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p></div><div class="output-specification"><p>If the required order of performing rules does not exist, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>Otherwise, print in the first line "<span class="tex-font-style-tt">YES</span>" (without the quotes), and in the second line — a sequence of <span class="tex-span">4<i>n</i></span> numbers from <span class="tex-span">1</span> to <span class="tex-span">4<i>n</i></span>, giving the numbers of the rules in the order they are applied. The sequence should be a permutation, that is, include each number from <span class="tex-span">1</span> to <span class="tex-span">4<i>n</i></span> exactly once.</p><p>If there are multiple possible variants, you are allowed to print any of them.</p></div>


## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 30 000</span>) — the number of servers of the social network.</p><p>Next <span class="tex-span">4<i>n</i></span> lines contain the rules of replicating processes, the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ 4<i>n</i></span>) of these lines as form <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) and describes rule <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> → (<i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>)</span>.</p><p>It is guaranteed that each number of a server from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs four times in the set of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, and eight times among a set that unites all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>.</p>


## Output

<p>If the required order of performing rules does not exist, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p><p>Otherwise, print in the first line "<span class="tex-font-style-tt">YES</span>" (without the quotes), and in the second line — a sequence of <span class="tex-span">4<i>n</i></span> numbers from <span class="tex-span">1</span> to <span class="tex-span">4<i>n</i></span>, giving the numbers of the rules in the order they are applied. The sequence should be a permutation, that is, include each number from <span class="tex-span">1</span> to <span class="tex-span">4<i>n</i></span> exactly once.</p><p>If there are multiple possible variants, you are allowed to print any of them.</p>


## Samples

```input1
2
1 2 2
1 2 2
1 2 2
1 2 2
2 1 1
2 1 1
2 1 1
2 1 1

```

```output1
YES
1 2 5 6 3 7 4 8

```






```input2
3
1 2 3
1 1 1
1 1 1
1 1 1
2 1 3
2 2 2
2 2 2
2 2 2
3 1 2
3 3 3
3 3 3
3 3 3

```

```output2
YES
2 3 4 6 7 8 10 11 12 1 5 9

```




## Note

<p><span class="tex-span"><sup class="upper-index">(1)</sup></span> To be extremely accurate, we should note that the amount of server memory is <span class="tex-span">1</span> GiB = <span class="tex-span">1024</span> MiB and processes require <span class="tex-span">100</span> MiB RAM where a gibibyte (GiB) is the amount of RAM of <span class="tex-span">2<sup class="upper-index">30</sup></span> bytes and a mebibyte (MiB) is the amount of RAM of <span class="tex-span">2<sup class="upper-index">20</sup></span> bytes.</p><p>In the first sample test the network uses two servers, each of which initially has four launched processes. In accordance with the rules of replication, each of the processes must be destroyed and twice run on another server. One of the possible answers is given in the statement: after applying rules <span class="tex-span">1</span> and <span class="tex-span">2</span> the first server will have <span class="tex-span">2</span> old running processes, and the second server will have <span class="tex-span">8</span> (<span class="tex-span">4</span> old and <span class="tex-span">4</span> new) processes. After we apply rules <span class="tex-span">5</span> and <span class="tex-span">6</span>, both servers will have <span class="tex-span">6</span> running processes (<span class="tex-span">2</span> old and <span class="tex-span">4</span> new). After we apply rules <span class="tex-span">3</span> and <span class="tex-span">7</span>, both servers will have <span class="tex-span">7</span> running processes (<span class="tex-span">1</span> old and <span class="tex-span">6</span> new), and after we apply rules <span class="tex-span">4</span> and <span class="tex-span">8</span>, each server will have <span class="tex-span">8</span> running processes. At no time the number of processes on a single server exceeds <span class="tex-span">9</span>.</p><p>In the second sample test the network uses three servers. On each server, three processes are replicated into two processes on the same server, and the fourth one is replicated in one process for each of the two remaining servers. As a result of applying rules <span class="tex-span">2, 3, 4, 6, 7, 8, 10, 11, 12</span> each server would have <span class="tex-span">7</span> processes (<span class="tex-span">6</span> old and <span class="tex-span">1</span> new), as a result of applying rules <span class="tex-span">1, 5, 9</span> each server will have <span class="tex-span">8</span> processes. At no time the number of processes on a single server exceeds <span class="tex-span">9</span>.</p>

