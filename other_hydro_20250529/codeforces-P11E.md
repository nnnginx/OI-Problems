## Description

<div><p>Jack has become a soldier now. Unfortunately, he has trouble with the drill. Instead of marching beginning with the left foot and then changing legs with each step, as ordered, he keeps repeating a sequence of steps, in which he sometimes makes the wrong steps or ！ horror of horrors! ！ stops for a while. For example, if Jack uses the sequence 'right, left, break', when the sergeant yells: 'Left! Right! Left! Right! Left! Right!', Jack first makes a step with the right foot, then one with the left foot, then he is confused and stops for a moment, then again - this time according to the order - starts with the right foot, then uses the left foot, then - to the sergeant's irritation - he stops to catch his breath, to incorrectly start with the right foot again... Marching this way, Jack will make the step that he is supposed to in the given moment in only one third of cases.</p><p>When the officers convinced him he should do something about it, Jack decided to modify the basic sequence of steps that he repeats. However, in order not to get too tired, he has decided that the only thing he'll do is adding any number of breaks in any positions of the original sequence (a break corresponds to stopping for the duration of one step). Of course, Jack can't make a step on the same foot twice in a row, if there is no pause between these steps. It is, however, not impossible that the sequence of steps he used so far is incorrect (it would explain a lot, actually).</p><p>Help Private Jack! Given the sequence of steps he keeps repeating, calculate the maximal percentage of time that he can spend marching correctly after adding some breaks to his scheme.</p></div><div class="input-specification"><p>The first line of input contains a sequence consisting only of characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>' and '<span class="tex-font-style-tt">X</span>', where '<span class="tex-font-style-tt">L</span>' corresponds to a step with the left foot, '<span class="tex-font-style-tt">R</span>' ！ with the right foot, and '<span class="tex-font-style-tt">X</span>' ！ to a break. The length of the sequence will not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Output the maximum percentage of time that Jack can spend marching correctly, <span class="tex-font-style-bf">rounded down to exactly six digits after the decimal point</span>.</p></div>


## Input

<p>The first line of input contains a sequence consisting only of characters '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>' and '<span class="tex-font-style-tt">X</span>', where '<span class="tex-font-style-tt">L</span>' corresponds to a step with the left foot, '<span class="tex-font-style-tt">R</span>' ！ with the right foot, and '<span class="tex-font-style-tt">X</span>' ！ to a break. The length of the sequence will not exceed <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p>


## Output

<p>Output the maximum percentage of time that Jack can spend marching correctly, <span class="tex-font-style-bf">rounded down to exactly six digits after the decimal point</span>.</p>


## Samples

```input1
X

```

```output1
0.000000

```






```input2
LXRR

```

```output2
50.000000

```




## Note

<p>In the second example, if we add two breaks to receive <span class="tex-font-style-tt">LXXRXR</span>, Jack will march: <span class="tex-font-style-tt">LXXRXRLXXRXRL</span>... instead of <span class="tex-font-style-tt">LRLRLRLRLRLRL</span>... and will make the correct step in half the cases. If we didn't add any breaks, the sequence would be incorrect ！ Jack can't step on his right foot twice in a row.</p>

