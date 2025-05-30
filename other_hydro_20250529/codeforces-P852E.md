## Description

<div><p>John has just bought a new car and is planning a journey around the country. Country has <span class="tex-span"><i>N</i></span> cities, some of which are connected by bidirectional roads. There are <span class="tex-span"><i>N</i> - 1</span> roads and every city is reachable from any other city. Cities are labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>N</i></span>.</p><p>John first has to select from which city he will start his journey. After that, he spends one day in a city and then travels to a randomly choosen city which is directly connected to his current one and which he has not yet visited. He does this until he can't continue obeying these rules.</p><p>To select the starting city, he calls his friend Jack for advice. Jack is also starting a big casino business and wants to open casinos in some of the cities (max <span class="tex-span">1</span> per city, maybe nowhere). Jack knows John well and he knows that if he visits a city with a casino, he will gamble exactly once before continuing his journey.</p><p>He also knows that if John enters a casino in a good mood, he will leave it in a bad mood and vice versa. Since he is John's friend, he wants him to be in a good mood at the moment when he finishes his journey. John is in a good mood before starting the journey.</p><p>In how many ways can Jack select a starting city for John and cities where he will build casinos such that no matter how John travels, he will be in a good mood at the end? Print answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>In the first line, a positive integer <span class="tex-span"><i>N</i> (1 ≤ <i>N</i> ≤ 100000)</span>, the number of cities. </p><p>In the next <span class="tex-span"><i>N</i> - 1</span> lines, two numbers <span class="tex-span"><i>a</i>,  <i>b</i> (1 ≤ <i>a</i>, <i>b</i> ≤ <i>N</i>)</span> separated by a single space meaning that cities <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are connected by a bidirectional road.</p></div><div class="output-specification"><p>Output one number, the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>In the first line, a positive integer <span class="tex-span"><i>N</i> (1 ≤ <i>N</i> ≤ 100000)</span>, the number of cities. </p><p>In the next <span class="tex-span"><i>N</i> - 1</span> lines, two numbers <span class="tex-span"><i>a</i>,  <i>b</i> (1 ≤ <i>a</i>, <i>b</i> ≤ <i>N</i>)</span> separated by a single space meaning that cities <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are connected by a bidirectional road.</p>

## Output

<p>Output one number, the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>

## Samples

```input1
2
1 2

```

```output1
4

```






```input2
3
1 2
2 3

```

```output2
10

```




## Note

<p>Example 1: If Jack selects city 1 as John's starting city, he can either build 0 casinos, so John will be happy all the time, or build a casino in both cities, so John would visit a casino in city 1, become unhappy, then go to city 2, visit a casino there and become happy and his journey ends there because he can't go back to city 1. If Jack selects city 2 for start, everything is symmetrical, so the answer is 4.</p><p>Example 2: If Jack tells John to start from city 1, he can either build casinos in 0 or 2 cities (total 4 possibilities). If he tells him to start from city 2, then John's journey will either contain cities 2 and 1 or 2 and 3. Therefore, Jack will either have to build no casinos, or build them in all three cities. With other options, he risks John ending his journey unhappy. Starting from 3 is symmetric to starting from 1, so in total we have <span class="tex-span">4 + 2 + 4 = 10</span> options.</p>
