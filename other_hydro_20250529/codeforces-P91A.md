## Description

<div><p>A newspaper is published in Walrusland. Its heading is <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, it consists of lowercase Latin letters. Fangy the little walrus wants to buy several such newspapers, cut out their headings, glue them one to another in order to get one big string. After that walrus erase several letters from this string in order to get a new word <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. It is considered that when Fangy erases some letter, there's no whitespace formed instead of the letter. That is, the string remains unbroken and it still only consists of lowercase Latin letters.</p><p>For example, the heading is "<span class="tex-font-style-tt">abc</span>". If we take two such headings and glue them one to the other one, we get "<span class="tex-font-style-tt">abcabc</span>". If we erase the letters on positions <span class="tex-span">1</span> and <span class="tex-span">5</span>, we get a word "<span class="tex-font-style-tt">bcac</span>".</p><p>Which least number of newspaper headings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span> will Fangy need to glue them, erase several letters and get word <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>?</p></div><div class="input-specification"><p>The input data contain two lines. The first line contain the heading <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, the second line contains the word <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. The lines only consist of lowercase Latin letters (<span class="tex-span">1 ≤ |<i>s</i><sub class="lower-index">1</sub>| ≤ 10<sup class="upper-index">4</sup>, 1 ≤ |<i>s</i><sub class="lower-index">2</sub>| ≤ 10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>If it is impossible to get the word <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> in the above-described manner, print "-1" (without the quotes). Otherwise, print the least number of newspaper headings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, which Fangy will need to receive the word <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>.</p></div>


## Input

<p>The input data contain two lines. The first line contain the heading <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, the second line contains the word <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>. The lines only consist of lowercase Latin letters (<span class="tex-span">1 ≤ |<i>s</i><sub class="lower-index">1</sub>| ≤ 10<sup class="upper-index">4</sup>, 1 ≤ |<i>s</i><sub class="lower-index">2</sub>| ≤ 10<sup class="upper-index">6</sup></span>).</p>


## Output

<p>If it is impossible to get the word <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span> in the above-described manner, print "-1" (without the quotes). Otherwise, print the least number of newspaper headings <span class="tex-span"><i>s</i><sub class="lower-index">1</sub></span>, which Fangy will need to receive the word <span class="tex-span"><i>s</i><sub class="lower-index">2</sub></span>.</p>


## Samples

```input1
abc
xyz

```

```output1
-1

```






```input2
abcd
dabc

```

```output2
2

```



