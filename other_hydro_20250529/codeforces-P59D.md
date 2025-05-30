## Description

<div><p>Recently personal training sessions have finished in the Berland State University Olympiad Programmer Training Centre. By the results of these training sessions teams are composed for the oncoming team contest season. Each team consists of three people. All the students of the Centre possess numbers from <span class="tex-span">1</span> to <span class="tex-span">3<i>n</i></span>, and all the teams possess numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The splitting of students into teams is performed in the following manner: while there are people who are not part of a team, a person with the best total score is chosen among them (the captain of a new team), this person chooses for himself two teammates from those who is left according to his list of priorities. The list of every person's priorities is represented as a permutation from <span class="tex-font-style-bf">the rest of</span> <span class="tex-span">3<i>n</i> - 1</span> students who attend the centre, besides himself.</p><p>You are given the results of personal training sessions which are a permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span">3<i>n</i></span>, where the <span class="tex-span"><i>i</i></span>-th number is the number of student who has won the <span class="tex-span"><i>i</i></span>-th place. No two students share a place. You are also given the arrangement of the already formed teams in the order in which they has been created. Your task is to determine the list of priorities for the student number <span class="tex-span"><i>k</i></span>. If there are several priority lists, choose the lexicographically minimal one.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which is the number of resulting teams. The second line contains <span class="tex-span">3<i>n</i></span> space-separated integers from <span class="tex-span">1</span> to <span class="tex-span">3<i>n</i></span> which are the results of personal training sessions. It is guaranteed that every student appears in the results exactly once.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines each containing three integers from <span class="tex-span">1</span> to <span class="tex-span">3<i>n</i></span> — each line describes the members of a given team. The members of one team can be listed in any order, but the teams themselves are listed in the order in which they were created. It is guaranteed that the arrangement is correct, that is that every student is a member of exactly one team and those teams could really be created from the given results using the method described above.</p><p>The last line contains number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 3<i>n</i></span>) which is the number of a student for who the list of priorities should be found.</p></div><div class="output-specification"><p>Print <span class="tex-span">3<i>n</i> - 1</span> numbers — the lexicographically smallest list of priorities for the student number <span class="tex-span"><i>k</i></span>. </p><p>The lexicographical comparison is performed by the standard &lt; operator in modern programming languages. The list <span class="tex-span"><i>a</i></span> is lexicographically less that the list <span class="tex-span"><i>b</i></span> if exists such an <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ 3<i>n</i></span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>. Note, that the list <span class="tex-font-style-tt">1 9 10</span> is lexicographically less than the list <span class="tex-font-style-tt">1 10 9</span>. That is, the comparison of lists is different from the comparison of lines.</p></div>


## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which is the number of resulting teams. The second line contains <span class="tex-span">3<i>n</i></span> space-separated integers from <span class="tex-span">1</span> to <span class="tex-span">3<i>n</i></span> which are the results of personal training sessions. It is guaranteed that every student appears in the results exactly once.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines each containing three integers from <span class="tex-span">1</span> to <span class="tex-span">3<i>n</i></span> — each line describes the members of a given team. The members of one team can be listed in any order, but the teams themselves are listed in the order in which they were created. It is guaranteed that the arrangement is correct, that is that every student is a member of exactly one team and those teams could really be created from the given results using the method described above.</p><p>The last line contains number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 3<i>n</i></span>) which is the number of a student for who the list of priorities should be found.</p>


## Output

<p>Print <span class="tex-span">3<i>n</i> - 1</span> numbers — the lexicographically smallest list of priorities for the student number <span class="tex-span"><i>k</i></span>. </p><p>The lexicographical comparison is performed by the standard &lt; operator in modern programming languages. The list <span class="tex-span"><i>a</i></span> is lexicographically less that the list <span class="tex-span"><i>b</i></span> if exists such an <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ 3<i>n</i></span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>. Note, that the list <span class="tex-font-style-tt">1 9 10</span> is lexicographically less than the list <span class="tex-font-style-tt">1 10 9</span>. That is, the comparison of lists is different from the comparison of lines.</p>


## Samples

```input1
3
5 4 1 2 6 3 7 8 9
5 6 2
9 3 4
1 7 8
4

```

```output1
2 3 5 6 9 1 7 8
```






```input2
3
5 4 1 2 6 3 7 8 9
5 6 2
9 3 4
1 7 8
8

```

```output2
1 2 3 4 5 6 7 9
```






```input3
2
4 1 3 2 5 6
4 6 5
1 2 3
4

```

```output3
5 6 1 2 3
```



