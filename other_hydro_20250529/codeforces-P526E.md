## Description

<div><p>Optimizing the amount of data transmitted via a network is an important and interesting part of developing any network application.</p><center> <img class="tex-graphics" src="./27346/file/aVhpt2hB.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In one secret game developed deep in the ZeptoLab company, the game universe consists of <span class="tex-span"><i>n</i></span> levels, located in a circle. You can get from level <span class="tex-span"><i>i</i></span> to levels <span class="tex-span"><i>i</i> - 1</span> and <span class="tex-span"><i>i</i> + 1</span>, also you can get from level <span class="tex-span">1</span> to level <span class="tex-span"><i>n</i></span> and vice versa. The map of the <span class="tex-span"><i>i</i></span>-th level description size is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> bytes.</p><p>In order to reduce the transmitted traffic, the game gets levels as follows. All the levels on the server are divided into <span class="tex-span"><i>m</i></span> groups and each time a player finds himself on one of the levels of a certain group for the first time, the server sends all levels of the group to the game client as a single packet. Thus, when a player travels inside the levels of a single group, the application doesn't need any new information. Due to the technical limitations the packet can contain an arbitrary number of levels but their total size mustn't exceed <span class="tex-span"><i>b</i></span> bytes, where <span class="tex-span"><i>b</i></span> is some positive integer constant.</p><p>Usual situation is that players finish levels one by one, that's why a decision was made to split <span class="tex-span"><i>n</i></span> levels into <span class="tex-span"><i>m</i></span> groups so that each group was a continuous segment containing multiple neighboring levels (also, the group can have two adjacent levels, <span class="tex-span"><i>n</i></span> and <span class="tex-span">1</span>). Specifically, if the descriptions of all levels have the total weight of at most <span class="tex-span"><i>b</i></span> bytes, then they can all be united into one group to be sent in a single packet.</p><p>Determine, what minimum number of groups do you need to make in order to organize the levels of the game observing the conditions above?</p><p>As developing a game is a long process and technology never stagnates, it is yet impossible to predict exactly what value will take constant value <span class="tex-span"><i>b</i></span> limiting the packet size when the game is out. That's why the developers ask you to find the answer for multiple values of <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 50</span>) — the number of levels in the game universe and the number of distinct values of <span class="tex-span"><i>b</i></span> that you need to process.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the sizes of the levels in bytes.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<img align="middle" class="tex-formula" src="./27346/file/uUkDV1Ia.png" style="max-width: 100.0%;max-height: 100.0%;">), determining the values of constant <span class="tex-span"><i>b</i></span>, for which you need to determine the answer.</p></div><div class="output-specification"><p>For each value of <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i></sub></span> from the input print on a single line integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>), determining the minimum number of groups to divide game levels into for transmission via network observing the given conditions. </p></div>


## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">6</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 50</span>) — the number of levels in the game universe and the number of distinct values of <span class="tex-span"><i>b</i></span> that you need to process.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the sizes of the levels in bytes.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<img align="middle" class="tex-formula" src="./27346/file/uUkDV1Ia.png" style="max-width: 100.0%;max-height: 100.0%;">), determining the values of constant <span class="tex-span"><i>b</i></span>, for which you need to determine the answer.</p>


## Output

<p>For each value of <span class="tex-span"><i>k</i><sub class="lower-index"><i>j</i></sub></span> from the input print on a single line integer <span class="tex-span"><i>m</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>), determining the minimum number of groups to divide game levels into for transmission via network observing the given conditions. </p>


## Samples

```input1
6 3
2 4 2 1 3 2
7
4
6

```

```output1
2
4
3

```




## Note

<p>In the test from the statement you can do in the following manner.</p><ul> <li> at <span class="tex-span"><i>b</i> = 7</span> you can divide into two segments: <span class="tex-span">2|421|32</span> (note that one of the segments contains the fifth, sixth and first levels); </li><li> at <span class="tex-span"><i>b</i> = 4</span> you can divide into four segments: <span class="tex-span">2|4|21|3|2</span>; </li><li> at <span class="tex-span"><i>b</i> = 6</span> you can divide into three segments: <span class="tex-span">24|21|32|</span>. </li></ul>

