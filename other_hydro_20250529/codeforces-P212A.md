## Description

<div><p>There is a developed network of flights between Berland and Beerland. All of them belong to the Berland state company BerAvia. Each flight connects some Berland city with some Beerland city. For each flight airplanes fly in both directions.</p><p>Changes are coming to Berland — the state decided to privatize BerAvia, namely, to sell out all flights to <span class="tex-span"><i>t</i></span> private companies. Each of these companies wants to get the maximal number of flights, so if the Berland flights are sold unevenly, Berland can be accused of partiality. Berland Government decided to sell the flights as evenly as possible between the <span class="tex-span"><i>t</i></span> companies.</p><p>The <span class="tex-font-style-it">unevenness</span> of the distribution of flights between companies is calculated as follows. For each city <span class="tex-span"><i>i</i></span> (both Berland and Beerland) we'll calculate the value of </p><center class="tex-equation"><img align="middle" class="tex-formula" src="./26067/file/pCm7RP0o.png" style="max-width: 100.0%;max-height: 100.0%;"></center> where <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub></span> is the number of flights from city <span class="tex-span"><i>i</i></span>, which belong to company <span class="tex-span"><i>j</i></span>. The sum of <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> for all cities in both countries is called the unevenness of the distribution. The distribution with the minimal unevenness is the most even one.<p>Help the Berland government come up with the most even distribution plan of selling flights.</p></div><div class="input-specification"><p>The first input line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>t</i> ≤ 200;1 ≤ <i>k</i> ≤ 5000</span>), where <span class="tex-span"><i>n</i>, <i>m</i></span> are the numbers of cities in Berland and Beerland, correspondingly, <span class="tex-span"><i>k</i></span> is the number of flights between them, and <span class="tex-span"><i>t</i></span> is the number of private companies. Next <span class="tex-span"><i>k</i></span> lines describe the flights, one per line, as pairs of positive integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the indexes of cities in Berland and Beerland, correspondingly, connected by the <span class="tex-span"><i>i</i></span>-th flight. There is at most one flight between any pair of cities, each flight connects cities of different countries. The cities in Berland are indexed from 1 to <span class="tex-span"><i>n</i></span>, and in Beerland — from 1 to <span class="tex-span"><i>m</i></span>.</p></div><div class="output-specification"><p>Print the unevenness of the sought plan on the first line. On the second line print a sequence of <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>t</i></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the index of the company that should buy the <span class="tex-span"><i>i</i></span>-th flight. Assume that the flights are indexed from 1 to <span class="tex-span"><i>k</i></span> in the order they appear in the input. If there are multiple solutions, print any of them.</p></div>


## Input

<p>The first input line contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>t</i> ≤ 200;1 ≤ <i>k</i> ≤ 5000</span>), where <span class="tex-span"><i>n</i>, <i>m</i></span> are the numbers of cities in Berland and Beerland, correspondingly, <span class="tex-span"><i>k</i></span> is the number of flights between them, and <span class="tex-span"><i>t</i></span> is the number of private companies. Next <span class="tex-span"><i>k</i></span> lines describe the flights, one per line, as pairs of positive integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;1 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>), where <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are the indexes of cities in Berland and Beerland, correspondingly, connected by the <span class="tex-span"><i>i</i></span>-th flight. There is at most one flight between any pair of cities, each flight connects cities of different countries. The cities in Berland are indexed from 1 to <span class="tex-span"><i>n</i></span>, and in Beerland — from 1 to <span class="tex-span"><i>m</i></span>.</p>


## Output

<p>Print the unevenness of the sought plan on the first line. On the second line print a sequence of <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ <i>t</i></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the index of the company that should buy the <span class="tex-span"><i>i</i></span>-th flight. Assume that the flights are indexed from 1 to <span class="tex-span"><i>k</i></span> in the order they appear in the input. If there are multiple solutions, print any of them.</p>


## Samples

```input1
3 5 8 2
1 4
1 3
3 3
1 2
1 1
2 1
1 5
2 2

```

```output1
4
2 1 2 1 2 1 2 2
```



