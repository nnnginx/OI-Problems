<p>Kinh_Can has a set of precious weights P<sub>1</sub>, P<sub>2</sub>, ..., P<sub>N</sub> in which the mass of the i<sup>th</sup> weight is P<sub>i</sub> = 3<sup>i-1</sup>, and a balance with 2 scales. On a nice day, Kinh_Can decided to show off his set of precious weights to his friends, and said that he can put them in equilibrium with any weight as long as its mass is not more than the mass of the sum of his weights. At first, his friends didn't believe, but after many trials they realized that Kinh_Can was right. In addition, while putting a thing whose mass is X on a scale, Kinh_Can could put right away the weights added on the 2 scales to keep their blance without any trial. 
With a random weight X (X is a natural number, X ¡Ù 0). Your task is to put weights on scales in order to keep the 2 scales' balance like Kinh_Can. The first scale initially weights X, and the second one weights 0.


</p><h3>Input</h3>
<p>Input has exactly one line consisting 2 numbers, the first is N and the second is X.

</p><h3>Output</h3>
<ul>
    <li>If there is no solution, you should write -1
    </li><li>If there is at least one solution for the problem, you should write exactly 2 lines:
        <ul>
            <li>The first line contains some numbers descripting the indices of the weights in the first disc
            </li><li>The second line contains some numbers description the indices of the weights in the second disc
            </li><li><b>Note:</b> One of 2 lines can be blank
        </li></ul>
</li></ul>

<h3>Constraints</h3>
<ul>
    <li>1 ¡Ü N ¡Ü 20
    </li><li>1 ¡Ü X ¡Ü 2000000000
</li></ul>

<h3>Example</h3>

<pre><b>Input 1:</b>
10 2

<b>Output 1:</b>
1
2

<b>Input 2:</b>
10 5

<b>Output 2:</b>
1 2
3

</pre>