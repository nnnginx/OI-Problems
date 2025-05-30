## Description

<div><p>You are given a straight half-line divided into segments of unit length, which we will call positions. The positions are numbered by positive integers that start with <span class="tex-span">1</span> from the end of half-line, i. e. <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and so on. The distance between the positions is the absolute difference between the respective numbers. </p><p>Laharl, Etna and Flonne occupy some positions on the half-line and they want to get to the position with the largest possible number. They are originally placed in different positions. </p><p>Each of the characters can perform each of the following actions <span class="tex-font-style-bf">no more than once</span>: </p><ul> <li> Move a certain distance. </li><li> Grab another character and lift him above the head. </li><li> Throw the lifted character a certain distance. </li></ul> <p>Each character has a <span class="tex-font-style-it">movement range</span> parameter. They can only move to free positions, assuming that distance between those positions doesn't exceed the movement range. </p><p>One character can lift another character if the distance between the two characters equals <span class="tex-span">1</span>, and no one already holds that another character. We can assume that the lifted character moves to the same position as the person who has lifted him, and the position in which he stood before becomes free. A lifted character cannot perform any actions and the character that holds him cannot walk. </p><p>Also, each character has a <span class="tex-font-style-it">throwing range</span> parameter. It is the distance at which this character can throw the one lifted above his head. He can only throw a character to a free position, and only when there is a lifted character. </p><p>We accept the situation when one person grabs another one who in his turn has the third character in his hands. This forms a "column" of three characters. For example, Laharl can hold Etna while Etna holds Flonne. In this case, Etna and the Flonne cannot perform any actions, and Laharl can only throw Etna (together with Flonne) at some distance. </p><p>Laharl, Etna and Flonne perform actions in any order. They perform actions in turns, that is no two of them can do actions at the same time.</p><p>Determine the maximum number of position at least one of the characters can reach. That is, such maximal number <span class="tex-span"><i>x</i></span> so that one of the characters can reach position <span class="tex-span"><i>x</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers: Laharl's position, his movement range and throwing range. The second and the third lines describe Etna's and Flonne's parameters correspondingly in the similar form. It is guaranteed that the three characters occupy distinct positions. All numbers in the input are between <span class="tex-span">1</span> and <span class="tex-span">10</span>, inclusive.</p></div><div class="output-specification"><p>Print a single number �� the maximum ordinal number of position which either Laharl, Etna or Flonne can reach.</p></div>


## Input

<p>The first line contains three integers: Laharl's position, his movement range and throwing range. The second and the third lines describe Etna's and Flonne's parameters correspondingly in the similar form. It is guaranteed that the three characters occupy distinct positions. All numbers in the input are between <span class="tex-span">1</span> and <span class="tex-span">10</span>, inclusive.</p>


## Output

<p>Print a single number �� the maximum ordinal number of position which either Laharl, Etna or Flonne can reach.</p>


## Samples

```input1
9 3 3
4 3 1
2 3 3

```

```output1
15
```




## Note

<p>Let us explain how to reach position <span class="tex-span">15</span> in the sample.</p><p>Initially Laharl occupies position <span class="tex-span">9</span>, Etna �� position <span class="tex-span">4</span> and Flonne �� position <span class="tex-span">2</span>.</p><p>First Laharl moves to position <span class="tex-span">6</span>.</p><p>Then Flonne moves to position <span class="tex-span">5</span> and grabs Etna.</p><p>Laharl grabs Flonne and throws to position <span class="tex-span">9</span>.</p><p>Flonne throws Etna to position <span class="tex-span">12</span>.</p><p>Etna moves to position <span class="tex-span">15</span>.</p>

