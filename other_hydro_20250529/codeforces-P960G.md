## Description

<div><p>Japate, while traveling through the forest of Mala, saw <span class="tex-span"><i>N</i></span> bags of gold lying in a row. Each bag has some <span class="tex-font-style-bf">distinct</span> weight of gold between <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span>. Japate can carry only one bag of gold with him, so he uses the following strategy to choose a bag.</p><p>Initially, he starts with an empty bag (zero weight). He considers the bags in some order. If the current bag has a higher weight than the bag in his hand, he picks the current bag.</p><p>Japate put the bags in some order. Japate realizes that he will pick <span class="tex-span"><i>A</i></span> bags, if he starts picking bags from the front, and will pick <span class="tex-span"><i>B</i></span> bags, if he starts picking bags from the back. By picking we mean replacing the bag in his hand with the current one.</p><p>Now he wonders how many permutations of bags are possible, in which he picks <span class="tex-span"><i>A</i></span> bags from the front and <span class="tex-span"><i>B</i></span> bags from back using the above strategy.</p><p>Since the answer can be very large, output it modulo <span class="tex-span">998244353</span>.</p></div><div class="input-specification"><p>The only line of input contains three space separated integers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> (<span class="tex-span">0 ≤ <i>A</i>, <i>B</i> ≤ <i>N</i></span>).</p></div><div class="output-specification"><p>Output a single integer — the number of valid permutations modulo <span class="tex-span">998244353</span>.</p></div>

## Input

<p>The only line of input contains three space separated integers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span>), <span class="tex-span"><i>A</i></span> and <span class="tex-span"><i>B</i></span> (<span class="tex-span">0 ≤ <i>A</i>, <i>B</i> ≤ <i>N</i></span>).</p>

## Output

<p>Output a single integer — the number of valid permutations modulo <span class="tex-span">998244353</span>.</p>

## Samples

```input1
1 1 1

```

```output1
1
```






```input2
2 1 1

```

```output2
0
```






```input3
2 2 1

```

```output3
1
```






```input4
5 2 2

```

```output4
22
```




## Note

<p>In sample case <span class="tex-span">1</span>, the only possible permutation is <span class="tex-span">[1]</span></p><p>In sample cases <span class="tex-span">2</span> and <span class="tex-span">3</span>, only two permutations of size <span class="tex-span">2</span> are possible:<span class="tex-span">{[1, 2], [2, 1]}</span>. The values of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> for first permutation is <span class="tex-span">2</span> and <span class="tex-span">1</span>, and for the second permutation these values are <span class="tex-span">1</span> and <span class="tex-span">2</span>. </p><p>In sample case <span class="tex-span">4</span>, out of 120 permutations of <span class="tex-span">[1, 2, 3, 4, 5]</span> possible, only 22 satisfy the given constraints of <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p>
