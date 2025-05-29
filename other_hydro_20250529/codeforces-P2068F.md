## Description

<div><p>When organizing a big event, organizers often handle side tasks outside their expertise. For example, the chief judge of EUC 2025 must find a name for the event's official mascot while satisfying certain constraints: </p><ul> <li> The name must include specific words as subsequences$^{\texttt{*}}$, such as the event name and location. You are given the list $s_1,\, s_2,\, \ldots,\, s_n$ of the $n$ required words. </li><li> The name must not contain as a subsequence$^{\texttt{*}}$ the name $t$ of last year's mascot. </li></ul> Please help the chief judge find a valid mascot name or determine that none exists.<p>$^{\texttt{*}}$ A string $x$ is a <span class="tex-font-style-underline">subsequence</span> of a string $y$ if $x$ can be obtained from $y$ by erasing some characters (at any positions) while keeping the remaining characters in the same order. For example, $\texttt{abc}$ is a subsequence of $\texttt{axbycz}$ but not of $\texttt{acbxyz}$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1\le n\le 200\,000$) �� the number of words that shall appear as subsequences.</p><p>The $i$-th of the following $n$ lines contains the string $s_i$ ($1\le |s_i| \le 200\,000$, $s_i$ consists of lowercase English letters) �� the $i$-th word in the list of words that shall appear as subsequences. The total length of these $n$ words is at most $200\,000$, i.e., $|s_1| + |s_2| + \cdots + |s_n| \le 200\,000$.</p><p>The last line contains the string $t$ ($1\le |t| \le 200\,000$, $t$ consists of lowercase English letters) �� the name of last year's mascot.</p></div><div class="output-specification"><p>Print $\texttt{YES}$ if there is a valid name for the mascot. Otherwise, print $\texttt{NO}$.</p><p>If there is a valid name, on the next line print a valid name. The string you print must have length at most $1\,000\,000$ and must consist of lowercase English letters. One can prove that if a valid name for the mascot exists, then there is one satisfying these additional constraints.</p><p>If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains an integer $n$ ($1\le n\le 200\,000$) �� the number of words that shall appear as subsequences.</p><p>The $i$-th of the following $n$ lines contains the string $s_i$ ($1\le |s_i| \le 200\,000$, $s_i$ consists of lowercase English letters) �� the $i$-th word in the list of words that shall appear as subsequences. The total length of these $n$ words is at most $200\,000$, i.e., $|s_1| + |s_2| + \cdots + |s_n| \le 200\,000$.</p><p>The last line contains the string $t$ ($1\le |t| \le 200\,000$, $t$ consists of lowercase English letters) �� the name of last year's mascot.</p>

## Output

<p>Print $\texttt{YES}$ if there is a valid name for the mascot. Otherwise, print $\texttt{NO}$.</p><p>If there is a valid name, on the next line print a valid name. The string you print must have length at most $1\,000\,000$ and must consist of lowercase English letters. One can prove that if a valid name for the mascot exists, then there is one satisfying these additional constraints.</p><p>If there are multiple solutions, print any of them.</p>





```input1|
2
porto
euc
prague
```




```input2|
6
credit
debit
money
rich
bank
capitalism
trap
```




```input3|
2
axiom
choice
io
```




```input4|
4
aaa
aab
abb
bbb
ba
```




```output1
YES
poretuco
```




```output2
YES
moncrdebditeychankpitalism
```




```output3
NO
```




```output4
YES
aaabbb
```



## Note

<p>In the <span class="tex-font-style-bf">first sample</span>, the words that must appear as subsequences are $\texttt{porto}$ and $\texttt{euc}$, while the word that must not appear as a subsequence is $\texttt{prague}$. There are many valid names for the mascot, e.g., $\texttt{poretuco}$ or $\texttt{xxxpppeortoucyyyy}$.</p><p>If $\texttt{poretuco}$ is chosen as the name of the mascot, observe that $\texttt{porto}$ and $\texttt{euc}$ are subsequences (highlighted in $\texttt{POReTucO}$ and $\texttt{porEtUCo}$, respectively), while $\texttt{prague}$ is not, as desired.</p><p>The string $\texttt{poretuc}$ is not a valid mascot name because it does not contain the word $\texttt{porto}$ as a subsequence. Also the string $\texttt{poretucoague}$ is not a valid mascot name because it contains $\texttt{prague}$ as a subsequence.</p>
