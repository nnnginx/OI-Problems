## Description

<div><p>Polycarpus has a finite sequence of opening and closing brackets. In order not to fall asleep in a lecture, Polycarpus is having fun with his sequence. He is able to perform two operations:</p><ul> <li> adding any bracket in any position (in the beginning, the end, or between any two existing brackets); </li><li> cyclic shift — moving the last bracket from the end of the sequence to the beginning. </li></ul><p>Polycarpus can apply any number of operations to his sequence and adding a cyclic shift in any order. As a result, he wants to get the correct bracket sequence of the minimum possible length. If there are several such sequences, Polycarpus is interested in the lexicographically smallest one. Help him find such a sequence.</p><p>A<span class="tex-font-style-it">correct bracket sequence</span> is a sequence of opening and closing brackets, from which you can get a correct arithmetic expression by adding characters "1" and "+" . Each opening bracket must correspond to a closed one. For example, the sequences "(())()", "()", "(()(()))" are correct and ")(", "(()" and "(()))(" are not.</p><p>The sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index"><i>n</i></sub></span> is lexicographically smaller than sequence <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> <span class="tex-span"><i>b</i><sub class="lower-index">2</sub>... <i>b</i><sub class="lower-index"><i>n</i></sub></span>, if there is such number <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, that<span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> = <i>b</i><sub class="lower-index"><i>k</i></sub></span> for <span class="tex-span">1 ≤ <i>k</i> &lt; <i>i</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>. Consider that "(" <span class="tex-span"> &lt; </span> ")".</p></div><div class="input-specification"><p>The first line contains Polycarpus's sequence consisting of characters "(" and ")". The length of a line is from <span class="tex-span">1</span> to <span class="tex-span">1 000 000</span>.</p></div><div class="output-specification"><p>Print a correct bracket sequence of the minimum length that Polycarpus can obtain by his operations. If there are multiple such sequences, print the lexicographically minimum one.</p></div>


## Input

<p>The first line contains Polycarpus's sequence consisting of characters "(" and ")". The length of a line is from <span class="tex-span">1</span> to <span class="tex-span">1 000 000</span>.</p>


## Output

<p>Print a correct bracket sequence of the minimum length that Polycarpus can obtain by his operations. If there are multiple such sequences, print the lexicographically minimum one.</p>


## Samples

```input1
()(())

```

```output1
(())()
```






```input2
()(

```

```output2
(())
```




## Note

<p>The sequence in the first example is already correct, but to get the lexicographically minimum answer, you need to perform four cyclic shift operations. In the second example you need to add a closing parenthesis between the second and third brackets and make a cyclic shift. You can first make the shift, and then add the bracket at the end.</p>

