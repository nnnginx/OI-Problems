## Description

<div><p>Petya loves hockey very much. One day, as he was watching a hockey match, he fell asleep. Petya dreamt of being appointed to change a hockey team's name. Thus, Petya was given the original team name <span class="tex-span"><i>w</i></span> and the collection of forbidden substrings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span>. All those strings consist of uppercase and lowercase Latin letters. String <span class="tex-span"><i>w</i></span> has the length of <span class="tex-span">|<i>w</i>|</span>, its characters are numbered from <span class="tex-span">1</span> to <span class="tex-span">|<i>w</i>|</span>.</p><p>First Petya should find all the occurrences of forbidden substrings in the <span class="tex-span"><i>w</i></span> string. During the search of substrings the case of letter shouldn't be taken into consideration. That is, strings "<span class="tex-font-style-tt">aBC</span>" and "<span class="tex-font-style-tt">ABc</span>" are considered equal.</p><p>After that Petya should perform the replacement of all letters covered by the occurrences. More formally: a letter in the position <span class="tex-span"><i>i</i></span> should be replaced by any other one if for position <span class="tex-span"><i>i</i></span> in string <span class="tex-span"><i>w</i></span> there exist pair of indices <span class="tex-span"><i>l</i>, <i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>i</i> ≤ <i>r</i> ≤ |<i>w</i>|</span>) such that substring <span class="tex-span"><i>w</i>[<i>l</i>&nbsp;...&nbsp;<i>r</i>]</span> is contained in the collection <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>n</i></sub></span>, when using case insensitive comparison. During the replacement the letter's case should remain the same. Petya is not allowed to replace the letters that aren't covered by any forbidden substring.</p><p>Letter <span class="tex-span"><i>letter</i></span> (uppercase or lowercase) is considered lucky for the hockey players. That's why Petya should perform the changes so that the <span class="tex-span"><i>letter</i></span> occurred in the resulting string as many times as possible. Help Petya to find such resulting string. If there are several such strings, find the one that comes first lexicographically.</p><p>Note that the process of replacements is not repeated, it occurs only once. That is, if after Petya's replacements the string started to contain new occurrences of bad substrings, Petya pays no attention to them.</p></div><div class="input-specification"><p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of forbidden substrings in the collection. Next <span class="tex-span"><i>n</i></span> lines contain these substrings. The next line contains string <span class="tex-span"><i>w</i></span>. All those <span class="tex-span"><i>n</i> + 1</span> lines are non-empty strings consisting of uppercase and lowercase Latin letters whose length does not exceed <span class="tex-span">100</span>. The last line contains a lowercase letter <span class="tex-span"><i>letter</i></span>.</p></div><div class="output-specification"><p>Output the only line — Petya's resulting string with the maximum number of letters <span class="tex-span"><i>letter</i></span>. If there are several answers then output the one that comes first lexicographically.</p><p>The lexicographical comparison is performed by the standard &lt; operator in modern programming languages. The line <span class="tex-span"><i>a</i></span> is lexicographically smaller than the line <span class="tex-span"><i>b</i></span>, if <span class="tex-span"><i>a</i></span> is a prefix of <span class="tex-span"><i>b</i></span>, or there exists such an <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ |<i>a</i>|</span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>. <span class="tex-span">|<i>a</i>|</span> stands for the length of string <span class="tex-span"><i>a</i></span>.</p></div>


## Input

<p>The first line contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of forbidden substrings in the collection. Next <span class="tex-span"><i>n</i></span> lines contain these substrings. The next line contains string <span class="tex-span"><i>w</i></span>. All those <span class="tex-span"><i>n</i> + 1</span> lines are non-empty strings consisting of uppercase and lowercase Latin letters whose length does not exceed <span class="tex-span">100</span>. The last line contains a lowercase letter <span class="tex-span"><i>letter</i></span>.</p>


## Output

<p>Output the only line — Petya's resulting string with the maximum number of letters <span class="tex-span"><i>letter</i></span>. If there are several answers then output the one that comes first lexicographically.</p><p>The lexicographical comparison is performed by the standard &lt; operator in modern programming languages. The line <span class="tex-span"><i>a</i></span> is lexicographically smaller than the line <span class="tex-span"><i>b</i></span>, if <span class="tex-span"><i>a</i></span> is a prefix of <span class="tex-span"><i>b</i></span>, or there exists such an <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ |<i>a</i>|</span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>. <span class="tex-span">|<i>a</i>|</span> stands for the length of string <span class="tex-span"><i>a</i></span>.</p>


## Samples

```input1
3
bers
ucky
elu
PetrLoveLuckyNumbers
t

```

```output1
PetrLovtTttttNumtttt

```






```input2
4
hello
party
abefglghjdhfgj
IVan
petrsmatchwin
a

```

```output2
petrsmatchwin

```






```input3
2
aCa
cba
abAcaba
c

```

```output3
abCacba

```



