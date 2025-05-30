## Description

<div><p>A group of university students wants to get to the top of a mountain to have a picnic there. For that they decided to use a cableway.</p><p>A cableway is represented by some cablecars, hanged onto some cable stations by a cable. A cable is scrolled cyclically between the first and the last cable stations (the first of them is located at the bottom of the mountain and the last one is located at the top). As the cable moves, the cablecar attached to it move as well.</p><p>The number of cablecars is divisible by three and they are painted three colors: red, green and blue, in such manner that after each red cablecar goes a green one, after each green cablecar goes a blue one and after each blue cablecar goes a red one. Each cablecar can transport no more than two people, the cablecars arrive with the periodicity of one minute (i. e. every minute) and it takes exactly <span class="tex-span">30</span> minutes for a cablecar to get to the top.</p><p>All students are divided into three groups: <span class="tex-span"><i>r</i></span> of them like to ascend only in the red cablecars, <span class="tex-span"><i>g</i></span> of them prefer only the green ones and <span class="tex-span"><i>b</i></span> of them prefer only the blue ones. A student never gets on a cablecar painted a color that he doesn't like,</p><p>The first cablecar to arrive (at the moment of time <span class="tex-span">0</span>) is painted red. Determine the least time it will take all students to ascend to the mountain top.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>g</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>r</i>, <i>g</i>, <i>b</i> ≤ 100</span>). It is guaranteed that <span class="tex-span"><i>r</i> + <i>g</i> + <i>b</i> &gt; 0</span>, it means that the group consists of at least one student. </p></div><div class="output-specification"><p>Print a single number — the minimal time the students need for the whole group to ascend to the top of the mountain.</p></div>


## Input

<p>The first line contains three integers <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>g</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>r</i>, <i>g</i>, <i>b</i> ≤ 100</span>). It is guaranteed that <span class="tex-span"><i>r</i> + <i>g</i> + <i>b</i> &gt; 0</span>, it means that the group consists of at least one student. </p>


## Output

<p>Print a single number — the minimal time the students need for the whole group to ascend to the top of the mountain.</p>


## Samples

```input1
1 3 2

```

```output1
34
```






```input2
3 2 1

```

```output2
33
```




## Note

<p>Let's analyze the first sample.</p><p>At the moment of time <span class="tex-span">0</span> a red cablecar comes and one student from the <span class="tex-span"><i>r</i></span> group get on it and ascends to the top at the moment of time <span class="tex-span">30</span>.</p><p>At the moment of time <span class="tex-span">1</span> a green cablecar arrives and two students from the <span class="tex-span"><i>g</i></span> group get on it; they get to the top at the moment of time <span class="tex-span">31</span>.</p><p>At the moment of time <span class="tex-span">2</span> comes the blue cablecar and two students from the <span class="tex-span"><i>b</i></span> group get on it. They ascend to the top at the moment of time <span class="tex-span">32</span>.</p><p>At the moment of time <span class="tex-span">3</span> a red cablecar arrives but the only student who is left doesn't like red and the cablecar leaves empty.</p><p>At the moment of time <span class="tex-span">4</span> a green cablecar arrives and one student from the <span class="tex-span"><i>g</i></span> group gets on it. He ascends to top at the moment of time <span class="tex-span">34</span>.</p><p>Thus, all the students are on the top, overall the ascension took exactly <span class="tex-span">34</span> minutes.</p>

