## Description

<div><p>Today, Yasser and Adel are at the shop buying cupcakes. There are $n$ cupcake types, arranged from $1$ to $n$ on the shelf, and there are infinitely many of each type. The tastiness of a cupcake of type $i$ is an integer $a_i$. There are both tasty and nasty cupcakes, so the tastiness can be positive, zero or negative.</p><p>Yasser, of course, wants to try them all, so he will buy exactly one cupcake of each type.</p><p>On the other hand, Adel will choose some segment $[l, r]$ $(1 \le l \le r \le n)$ that does not include all of cupcakes (he can't choose $[l, r] = [1, n]$) and buy exactly one cupcake of each of types $l, l + 1, \dots, r$.</p><p>After that they will compare the total tastiness of the cupcakes each of them have bought. Yasser will be happy if the total tastiness of cupcakes he buys is <span class="tex-font-style-bf">strictly</span> greater than the total tastiness of cupcakes Adel buys <span class="tex-font-style-bf">regardless of Adel's choice</span>.</p><p>For example, let the tastinesses of the cupcakes be $[7, 4, -1]$. Yasser will buy all of them, the total tastiness will be $7 + 4 - 1 = 10$. Adel can choose segments $[7], [4], [-1], [7, 4]$ or $[4, -1]$, their total tastinesses are $7, 4, -1, 11$ and $3$, respectively. Adel can choose segment with tastiness $11$, and as $10$ is not strictly greater than $11$, Yasser won't be happy :(</p><p>Find out if Yasser will be happy after visiting the shop.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$), where $a_i$ represents the tastiness of the $i$-th type of cupcake.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print "<span class="tex-font-style-tt">YES</span>", if the total tastiness of cupcakes Yasser buys will always be <span class="tex-font-style-bf">strictly</span> greater than the total tastiness of cupcakes Adel buys regardless of Adel's choice. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows.</p><p>The first line of each test case contains $n$ ($2 \le n \le 10^5$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ ($-10^9 \le a_i \le 10^9$), where $a_i$ represents the tastiness of the $i$-th type of cupcake.</p><p>It is guaranteed that the sum of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case, print "<span class="tex-font-style-tt">YES</span>", if the total tastiness of cupcakes Yasser buys will always be <span class="tex-font-style-bf">strictly</span> greater than the total tastiness of cupcakes Adel buys regardless of Adel's choice. Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>

## Samples

```input1
3
4
1 2 3 4
3
7 4 -1
3
5 -5 5
```

```output1
YES
NO
NO
```




## Note

<p>In the first example, the total tastiness of any segment Adel can choose is less than the total tastiness of all cupcakes.</p><p>In the second example, Adel will choose the segment $[1, 2]$ with total tastiness $11$, which is not less than the total tastiness of all cupcakes, which is $10$.</p><p>In the third example, Adel can choose the segment $[3, 3]$ with total tastiness of $5$. Note that Yasser's cupcakes' total tastiness is also $5$, so in that case, the total tastiness of Yasser's cupcakes isn't strictly greater than the total tastiness of Adel's cupcakes.</p>
