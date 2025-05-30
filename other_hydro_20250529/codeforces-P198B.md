## Description

<div><p>Vasya plays a computer game with ninjas. At this stage Vasya's ninja should get out of a deep canyon.</p><p>The canyon consists of two vertical parallel walls, their height is <span class="tex-span"><i>n</i></span> meters. Let's imagine that we split these walls into <span class="tex-span">1</span> meter-long areas and number them with positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from bottom to top. Some areas are safe and the ninja can climb them. Others are spiky and ninja can't be there. Let's call such areas <span class="tex-font-style-it">dangerous</span>.</p><p>Initially the ninja is on the lower area of the left wall. He can use each second to perform one of the following actions: </p><ul> <li> climb one area up; </li><li> climb one area down; </li><li> jump to the opposite wall. That gets the ninja to the area that is exactly <span class="tex-span"><i>k</i></span> meters higher than the area he jumped from. More formally, if before the jump the ninja is located at area <span class="tex-span"><i>x</i></span> of one wall, then after the jump he is located at area <span class="tex-span"><i>x</i> + <i>k</i></span> of the other wall. </li></ul><p>If at some point of time the ninja tries to get to an area with a number larger than <span class="tex-span"><i>n</i></span>, then we can assume that the ninja got out of the canyon.</p><p>The canyon gets flooded and each second the water level raises one meter. Initially the water level is at the lower border of the first area. Ninja cannot be on the area covered by water. We can assume that the ninja and the water "move in turns" — first the ninja performs some action, then the water raises for one meter, then the ninja performs one more action and so on.</p><p>The level is considered completed if the ninja manages to get out of the canyon.</p><p>After several failed attempts Vasya started to doubt whether it is possible to complete the level at all. Help him answer the question.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the height of the canyon and the height of ninja's jump, correspondingly.</p><p>The second line contains the description of the left wall — a string with the length of <span class="tex-span"><i>n</i></span> characters. The <span class="tex-span"><i>i</i></span>-th character represents the state of the <span class="tex-span"><i>i</i></span>-th wall area: character "<span class="tex-font-style-tt">X</span>" represents a dangerous area and character "<span class="tex-font-style-tt">-</span>" represents a safe area.</p><p>The third line describes the right wall in the same format.</p><p>It is guaranteed that the first area of the left wall is not dangerous.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if the ninja can get out from the canyon, otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>


## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>) — the height of the canyon and the height of ninja's jump, correspondingly.</p><p>The second line contains the description of the left wall — a string with the length of <span class="tex-span"><i>n</i></span> characters. The <span class="tex-span"><i>i</i></span>-th character represents the state of the <span class="tex-span"><i>i</i></span>-th wall area: character "<span class="tex-font-style-tt">X</span>" represents a dangerous area and character "<span class="tex-font-style-tt">-</span>" represents a safe area.</p><p>The third line describes the right wall in the same format.</p><p>It is guaranteed that the first area of the left wall is not dangerous.</p>


## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if the ninja can get out from the canyon, otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>


## Samples

```input1
7 3
---X--X
-X--XX-

```

```output1
YES

```






```input2
6 2
--X-X-
X--XX-

```

```output2
NO

```




## Note

<p>In the first sample the ninja should first jump to the right wall, then go one meter down along the right wall, then jump to the left wall. The next jump can get the ninja from the canyon. </p><p>In the second sample there's no way the ninja can get out of the canyon.</p>

