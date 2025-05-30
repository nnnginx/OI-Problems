## Description

<div><p>After his wife's tragic death, Eurydice, Orpheus descended to the realm of death to see her. Reaching its gates was uneasy, but passing through them proved to be even more challenging. Mostly because of Cerberus, the three-headed hound of Hades. </p><p>Orpheus, a famous poet, and musician plans to calm Cerberus with his poetry and safely walk past him. He created a very peculiar poem for Cerberus. It consists only of lowercase English letters. </p><p>We call a poem's substring a palindrome if and only if it reads the same backwards and forwards. A string $a$ is a substring of a string $b$ if $a$ can be obtained from $b$ by deleting several (possibly zero or all) characters from the beginning and several (possibly zero or all) characters from the end.</p><p>Unfortunately, Cerberus dislikes palindromes of length greater than $1$. For example in the poem <span class="tex-font-style-tt">abaa</span> the hound of Hades wouldn't like substrings <span class="tex-font-style-tt">aba</span> and <span class="tex-font-style-tt">aa</span>.</p><p>Orpheus can only calm Cerberus if the hound likes his poetry. That's why he wants to change his poem so that it does not contain any palindrome substrings of length <span class="tex-font-style-bf">greater than $1$</span>.</p><p>Orpheus can modify the poem by replacing a letter at any position with any lowercase English letter. He can use this operation arbitrarily many times (possibly zero). Since there can be many palindromes in his poem, he may have to make some corrections. But how many, exactly? Given the poem, determine the minimal number of letters that have to be changed so that the poem does not contain any palindromes of length greater than $1$.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 10^5$) denoting the number of test cases, then $t$ test cases follow.</p><p>The first and only line of each test case contains a non-empty string of lowercase English letters, Orpheus' poem.</p><p>The sum of the length of Orpheus' poems in all test cases will not exceed $10^5$.</p></div><div class="output-specification"><p>You should output $t$ lines, $i$-th line should contain a single integer, answer to the $i$-th test case.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \leq t \leq 10^5$) denoting the number of test cases, then $t$ test cases follow.</p><p>The first and only line of each test case contains a non-empty string of lowercase English letters, Orpheus' poem.</p><p>The sum of the length of Orpheus' poems in all test cases will not exceed $10^5$.</p>

## Output

<p>You should output $t$ lines, $i$-th line should contain a single integer, answer to the $i$-th test case.</p>

## Samples

```input1
7
babba
abaac
codeforces
zeroorez
abcdcba
bbbbbbb
a
```

```output1
1
1
0
1
1
4
0
```




## Note

<p>In the first test case, we can replace the third character with <span class="tex-font-style-tt">c</span> and obtain a palindrome-less poem <span class="tex-font-style-tt">bacba</span>.</p><p>In the second test case, we can replace the third character with <span class="tex-font-style-tt">d</span> and obtain a palindrome-less poem <span class="tex-font-style-tt">abdac</span>.</p><p>In the third test case, the initial poem already doesn't contain any palindromes, so Orpheus doesn't need to change anything there.</p>
