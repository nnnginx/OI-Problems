## Description

<div><p>Some time ago Lesha found an entertaining string $s$ consisting of lowercase English letters. Lesha immediately developed an unique algorithm for this string and shared it with you. The algorithm is as follows.</p><p>Lesha chooses an arbitrary (possibly zero) number of pairs on positions $(i, i + 1)$ in such a way that the following conditions are satisfied: </p><ul> <li> for each pair $(i, i + 1)$ the inequality $0 \le i &lt; |s| - 1$ holds; </li><li> for each pair $(i, i + 1)$ the equality $s_i = s_{i + 1}$ holds; </li><li> there is no index that is contained in more than one pair. </li></ul> After that Lesha removes all characters on indexes contained in these pairs and the algorithm is over. <p>Lesha is interested in the lexicographically smallest strings he can obtain by applying the algorithm to the suffixes of the given string.</p></div><div class="input-specification"><p>The only line contains the string $s$ ($1 \le |s| \le 10^5$) �� the initial string consisting of lowercase English letters only.</p></div><div class="output-specification"><p>In $|s|$ lines print the lengths of the answers and the answers themselves, starting with the answer for the longest suffix. The output can be large, so, when some answer is longer than $10$ characters, instead print the first $5$ characters, then "<span class="tex-font-style-tt">...</span>", then the last $2$ characters of the answer.</p></div>

## Input

<p>The only line contains the string $s$ ($1 \le |s| \le 10^5$) �� the initial string consisting of lowercase English letters only.</p>

## Output

<p>In $|s|$ lines print the lengths of the answers and the answers themselves, starting with the answer for the longest suffix. The output can be large, so, when some answer is longer than $10$ characters, instead print the first $5$ characters, then "<span class="tex-font-style-tt">...</span>", then the last $2$ characters of the answer.</p>

## Samples

```input1
abcdd
```

```output1
3 abc
2 bc
1 c
0 
1 d
```






```input2
abbcdddeaaffdfouurtytwoo
```

```output2
18 abbcd...tw
17 bbcdd...tw
16 bcddd...tw
15 cddde...tw
14 dddea...tw
13 ddeaa...tw
12 deaad...tw
11 eaadf...tw
10 aadfortytw
9 adfortytw
8 dfortytw
9 fdfortytw
8 dfortytw
7 fortytw
6 ortytw
5 rtytw
6 urtytw
5 rtytw
4 tytw
3 ytw
2 tw
1 w
0 
1 o
```




## Note

<p>Consider the first example.</p><ul> <li> The longest suffix is the whole string "<span class="tex-font-style-tt">abcdd</span>". Choosing one pair $(4, 5)$, Lesha obtains "<span class="tex-font-style-tt">abc</span>". </li><li> The next longest suffix is "<span class="tex-font-style-tt">bcdd</span>". Choosing one pair $(3, 4)$, we obtain "<span class="tex-font-style-tt">bc</span>". </li><li> The next longest suffix is "<span class="tex-font-style-tt">cdd</span>". Choosing one pair $(2, 3)$, we obtain "<span class="tex-font-style-tt">c</span>". </li><li> The next longest suffix is "<span class="tex-font-style-tt">dd</span>". Choosing one pair $(1, 2)$, we obtain "<span class="tex-font-style-tt"></span>" (an empty string). </li><li> The last suffix is the string "<span class="tex-font-style-tt">d</span>". No pair can be chosen, so the answer is "<span class="tex-font-style-tt">d</span>". </li></ul><p>In the second example, for the longest suffix "<span class="tex-font-style-tt">abbcdddeaaffdfouurtytwoo</span>" choose three pairs $(11, 12)$, $(16, 17)$, $(23, 24)$ and we obtain "<span class="tex-font-style-tt">abbcdddeaadfortytw</span>"</p>
