## Description

<div><p>Malek has recently found a treasure map. While he was looking for a treasure he found a locked door. There was a string <span class="tex-span"><i>s</i></span> written on the door consisting of characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' and '<span class="tex-font-style-tt">#</span>'. Below there was a manual on how to open the door. After spending a long time Malek managed to decode the manual and found out that the goal is to replace each '<span class="tex-font-style-tt">#</span>' with one or more '<span class="tex-font-style-tt">)</span>' characters so that the final string becomes <span class="tex-font-style-underline">beautiful</span>. </p><p>Below there was also written that a string is called <span class="tex-font-style-underline">beautiful</span> if for each <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ |<i>s</i>|</span>) there are no more '<span class="tex-font-style-tt">)</span>' characters than '<span class="tex-font-style-tt">(</span>' characters among the first <span class="tex-span"><i>i</i></span> characters of <span class="tex-span"><i>s</i></span> and also the total number of '<span class="tex-font-style-tt">(</span>' characters is equal to the total number of '<span class="tex-font-style-tt">)</span>' characters. </p><p>Help Malek open the door by telling him for each '<span class="tex-font-style-tt">#</span>' character how many '<span class="tex-font-style-tt">)</span>' characters he must replace it with.</p></div><div class="input-specification"><p>The first line of the input contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>). Each character of this string is one of the characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' or '<span class="tex-font-style-tt">#</span>'. It is guaranteed that <span class="tex-span"><i>s</i></span> contains at least one '<span class="tex-font-style-tt">#</span>' character.</p></div><div class="output-specification"><p>If there is no way of replacing '<span class="tex-font-style-tt">#</span>' characters which leads to a beautiful string print <span class="tex-span"> - 1</span>. Otherwise for each character '<span class="tex-font-style-tt">#</span>' print a separate line containing a positive integer, the number of '<span class="tex-font-style-tt">)</span>' characters this character must be replaced with.</p><p><span class="tex-font-style-bf">If there are several possible answers, you may output any of them.</span></p></div>


## Input

<p>The first line of the input contains a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>). Each character of this string is one of the characters '<span class="tex-font-style-tt">(</span>', '<span class="tex-font-style-tt">)</span>' or '<span class="tex-font-style-tt">#</span>'. It is guaranteed that <span class="tex-span"><i>s</i></span> contains at least one '<span class="tex-font-style-tt">#</span>' character.</p>


## Output

<p>If there is no way of replacing '<span class="tex-font-style-tt">#</span>' characters which leads to a beautiful string print <span class="tex-span"> - 1</span>. Otherwise for each character '<span class="tex-font-style-tt">#</span>' print a separate line containing a positive integer, the number of '<span class="tex-font-style-tt">)</span>' characters this character must be replaced with.</p><p><span class="tex-font-style-bf">If there are several possible answers, you may output any of them.</span></p>


## Samples

```input1
(((#)((#)

```

```output1
1
2

```






```input2
()((#((#(#()

```

```output2
2
2
1
```






```input3
#

```

```output3
-1

```






```input4
(#)

```

```output4
-1

```




## Note

<p><span class="tex-span">|<i>s</i>|</span> denotes the length of the string <span class="tex-span"><i>s</i></span>.</p>

