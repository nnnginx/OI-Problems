## Description

<div><p>Do you like summer? Residents of Berland do. They especially love eating ice cream in the hot summer. So this summer day a large queue of <span class="tex-span"><i>n</i></span> Berland residents lined up in front of the ice cream stall. We know that each of them has a certain amount of berland dollars with them. The residents of Berland are nice people, so each person agrees to swap places with the person right behind him for just 1 dollar. More formally, if person <span class="tex-span"><i>a</i></span> stands just behind person <span class="tex-span"><i>b</i></span>, then person <span class="tex-span"><i>a</i></span> can pay person <span class="tex-span"><i>b</i></span> 1 dollar, then <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> get swapped. Of course, if person <span class="tex-span"><i>a</i></span> has zero dollars, he can not swap places with person <span class="tex-span"><i>b</i></span>.</p><p>Residents of Berland are strange people. In particular, they get upset when there is someone with a <span class="tex-font-style-it">strictly smaller</span> sum of money in the line in front of them.</p><p>Can you help the residents of Berland form such order in the line so that they were all <span class="tex-font-style-it">happy</span>? A <span class="tex-font-style-it">happy</span> resident is the one who stands first in the line or the one in front of who another resident stands with <span class="tex-font-style-it">not less</span> number of dollars. Note that the people of Berland are people of honor and they agree to swap places only in the manner described above.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of residents who stand in the line.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of Berland dollars of a man standing on the <span class="tex-span"><i>i</i></span>-th position in the line. The positions are numbered starting from the <span class="tex-font-style-it">end</span> of the line. </p></div><div class="output-specification"><p>If it is impossible to make all the residents happy, print <span class="tex-font-style-tt">":("</span> without the quotes. Otherwise, print in the single line <span class="tex-span"><i>n</i></span> space-separated integers, the <span class="tex-span"><i>i</i></span>-th of them must be equal to the number of money of the person on position <span class="tex-span"><i>i</i></span> in the new line. If there are multiple answers, print any of them.</p></div>


## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>) — the number of residents who stand in the line.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of Berland dollars of a man standing on the <span class="tex-span"><i>i</i></span>-th position in the line. The positions are numbered starting from the <span class="tex-font-style-it">end</span> of the line. </p>


## Output

<p>If it is impossible to make all the residents happy, print <span class="tex-font-style-tt">":("</span> without the quotes. Otherwise, print in the single line <span class="tex-span"><i>n</i></span> space-separated integers, the <span class="tex-span"><i>i</i></span>-th of them must be equal to the number of money of the person on position <span class="tex-span"><i>i</i></span> in the new line. If there are multiple answers, print any of them.</p>


## Samples

```input1
2
11 8

```

```output1
9 10
```






```input2
5
10 9 7 10 6

```

```output2
:(

```






```input3
3
12 3 3

```

```output3
4 4 10
```




## Note

<p>In the first sample two residents should swap places, after that the first resident has 10 dollars and he is at the head of the line and the second resident will have 9 coins and he will be at the end of the line. </p><p>In the second sample it is impossible to achieve the desired result.</p><p>In the third sample the first person can swap with the second one, then they will have the following numbers of dollars: <span class="tex-span">4 11 3</span>, then the second person (in the new line) swaps with the third one, and the resulting numbers of dollars will equal to: <span class="tex-span">4 4 10</span>. In this line everybody will be happy.</p>

