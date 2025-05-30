## Description

<div><p>After the Search Ultimate program that searched for strings in a text failed, Igor K. got to think: "Why on Earth does my program work so slowly?" As he double-checked his code, he said: "My code contains no errors, yet I know how we will improve Search Ultimate!" and took a large book from the shelves. The book read "Azembler. Principally New Approach".</p><p>Having carefully thumbed through the book, Igor K. realised that, as it turns out, you can multiply the numbers dozens of times faster. "Search Ultimate will be faster than it has ever been!" — the fellow shouted happily and set to work.</p><p>Let us now clarify what Igor's idea was. The thing is that the code that was generated by a compiler was far from perfect. Standard multiplying does work slower than with the trick the book mentioned.</p><p>The Azembler language operates with 26 registers (eax, ebx, ..., ezx) and two commands: </p><ul> <li> [<span class="tex-span"><i>x</i></span>] — returns the value located in the address <span class="tex-span"><i>x</i></span>. For example, [eax] returns the value that was located in the address, equal to the value in the register eax. </li><li> lea <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> — assigns to the register <span class="tex-span"><i>x</i></span>, indicated as the first operand, the second operand's address. Thus, for example, the "lea ebx, [eax]" command will write in the ebx register the content of the eax register: first the [eax] operation will be fulfilled, the result of it will be some value that lies in the address written in eax. But we do not need the value — the next operation will be lea, that will take the [eax] address, i.e., the value in the eax register, and will write it in ebx. </li></ul><p>On the first thought the second operation seems meaningless, but as it turns out, it is acceptable to write the operation as </p><p>lea ecx, [eax + ebx],</p><p>lea ecx, [k*eax]</p><p>or even</p><p>lea ecx, [ebx + k*eax],</p><p>where k = 1, 2, 4 or 8.</p><p>As a result, the register ecx will be equal to the numbers eax + ebx, k*eax and ebx + k*eax correspondingly. However, such operation is fulfilled many times, dozens of times faster that the usual multiplying of numbers. And using several such operations, one can very quickly multiply some number by some other one. Of course, instead of eax, ebx and ecx you are allowed to use any registers.</p><p>For example, let the eax register contain some number that we should multiply by 41. It takes us 2 lines:</p><p>lea ebx, [eax + 4*eax] // now ebx = 5*eax</p><p>lea eax, [eax + 8*ebx] // now eax = eax + 8*ebx = 41*eax</p><p>Igor K. got interested in the following question: what is the minimum number of lea operations needed to multiply by the given number <span class="tex-span"><i>n</i></span> and how to do it? Your task is to help him.</p><p>Consider that at the initial moment of time eax contains a number that Igor K. was about to multiply by <span class="tex-span"><i>n</i></span>, and the registers from ebx to ezx contain number 0. At the final moment of time the result can be located in any register.</p></div><div class="input-specification"><p>The input data contain the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 255</span>), which Igor K. is about to multiply.</p></div><div class="output-specification"><p>On the first line print number <span class="tex-span"><i>p</i></span>, which represents the minimum number of lea operations, needed to do that. Then print the program consisting of <span class="tex-span"><i>p</i></span> commands, performing the operations. It is guaranteed that such program exists for any <span class="tex-span"><i>n</i></span> from 1 to 255.</p><p>Use precisely the following format of commands (here <span class="tex-span"><i>k</i></span> is equal to 1, 2, 4 or 8, and <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> are any, even coinciding registers):</p><p>lea x, [y]</p><p>lea x, [y + z]</p><p>lea x, [k*y]</p><p>lea x, [y + k*z]</p><p>Please note that <span class="tex-font-style-bf">extra spaces at the end of a command are unacceptable</span>.</p></div>


## Input

<p>The input data contain the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 255</span>), which Igor K. is about to multiply.</p>


## Output

<p>On the first line print number <span class="tex-span"><i>p</i></span>, which represents the minimum number of lea operations, needed to do that. Then print the program consisting of <span class="tex-span"><i>p</i></span> commands, performing the operations. It is guaranteed that such program exists for any <span class="tex-span"><i>n</i></span> from 1 to 255.</p><p>Use precisely the following format of commands (here <span class="tex-span"><i>k</i></span> is equal to 1, 2, 4 or 8, and <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> are any, even coinciding registers):</p><p>lea x, [y]</p><p>lea x, [y + z]</p><p>lea x, [k*y]</p><p>lea x, [y + k*z]</p><p>Please note that <span class="tex-font-style-bf">extra spaces at the end of a command are unacceptable</span>.</p>


## Samples

```input1
41

```

```output1
2
lea ebx, [eax + 4*eax]
lea ecx, [eax + 8*ebx]

```






```input2
2

```

```output2
1
lea ebx, [eax + eax]

```






```input3
4

```

```output3
1
lea ebx, [4*eax]

```



