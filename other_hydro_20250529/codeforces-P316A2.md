## Description

<div><p>Special Agent Smart Beaver works in a secret research department of ABBYY. He's been working there for a long time and is satisfied with his job, as it allows him to eat out in the best restaurants and order the most expensive and exotic wood types there. </p><p>The content special agent has got an important task: to get the latest research by British scientists on the English Language. These developments are encoded and stored in a large safe. The Beaver's teeth are strong enough, so the authorities assured that upon arriving at the place the beaver won't have any problems with opening the safe.</p><p>And he finishes his aspen sprig and leaves for this important task. Of course, the Beaver arrived at the location without any problems, but alas. He can't open the safe with his strong and big teeth. At this point, the Smart Beaver get a call from the headquarters and learns that opening the safe with the teeth is not necessary, as a reliable source has sent the following information: the safe code consists of digits and has no leading zeroes. There also is a special hint, which can be used to open the safe. The hint is string <span class="tex-span"><i>s</i></span> with the following structure:</p><ul> <li> if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> = "<span class="tex-font-style-tt">?</span>", then the digit that goes <span class="tex-span"><i>i</i></span>-th in the safe code can be anything (between <span class="tex-span">0</span> to <span class="tex-span">9</span>, inclusively); </li><li> if <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> is a digit (between <span class="tex-span">0</span> to <span class="tex-span">9</span>, inclusively), then it means that there is digit <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> on position <span class="tex-span"><i>i</i></span> in code; </li><li> if the string contains letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">J</span>", then all positions with the same letters must contain the same digits and the positions with distinct letters must contain distinct digits. </li><li> The length of the safe code coincides with the length of the hint. </li></ul><p>For example, hint "<span class="tex-font-style-tt">?JGJ9</span>" has such matching safe code variants: "<span class="tex-font-style-tt">51919</span>", "<span class="tex-font-style-tt">55959</span>", "<span class="tex-font-style-tt">12329</span>", "<span class="tex-font-style-tt">93539</span>" and so on, and has wrong variants such as: "<span class="tex-font-style-tt">56669</span>", "<span class="tex-font-style-tt">00111</span>", "<span class="tex-font-style-tt">03539</span>" and "<span class="tex-font-style-tt">13666</span>".</p><p>After receiving such information, the authorities change the plan and ask the special agents to work quietly and gently and not to try to open the safe by mechanical means, and try to find the password using the given hint.</p><p>At a special agent school the Smart Beaver was the fastest in his platoon finding codes for such safes, but now he is not in that shape: the years take their toll ... Help him to determine the number of possible variants of the code to the safe, matching the given hint. After receiving this information, and knowing his own speed of entering codes, the Smart Beaver will be able to determine whether he will have time for tonight's show "Beavers are on the trail" on his favorite TV channel, or he should work for a sleepless night...</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> — the hint to the safe code. String <span class="tex-span"><i>s</i></span> consists of the following characters: <span class="tex-font-style-tt">?, 0-9, A-J</span>. It is guaranteed that the first character of string <span class="tex-span"><i>s</i></span> doesn't equal to character <span class="tex-span">0</span>.</p><p>The input limits for scoring 30 points are (subproblem A1): </p><ul> <li> <span class="tex-span">1 ≤ |<i>s</i>| ≤ 5</span>. </li></ul><p>The input limits for scoring 100 points are (subproblems A1+A2): </p><ul> <li> <span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>. </li></ul><p>Here <span class="tex-span">|<i>s</i>|</span> means the length of string <span class="tex-span"><i>s</i></span>.</p></div><div class="output-specification"><p>Print the number of codes that match the given hint.</p></div>


## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> — the hint to the safe code. String <span class="tex-span"><i>s</i></span> consists of the following characters: <span class="tex-font-style-tt">?, 0-9, A-J</span>. It is guaranteed that the first character of string <span class="tex-span"><i>s</i></span> doesn't equal to character <span class="tex-span">0</span>.</p><p>The input limits for scoring 30 points are (subproblem A1): </p><ul> <li> <span class="tex-span">1 ≤ |<i>s</i>| ≤ 5</span>. </li></ul><p>The input limits for scoring 100 points are (subproblems A1+A2): </p><ul> <li> <span class="tex-span">1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">5</sup></span>. </li></ul><p>Here <span class="tex-span">|<i>s</i>|</span> means the length of string <span class="tex-span"><i>s</i></span>.</p>


## Output

<p>Print the number of codes that match the given hint.</p>


## Samples

```input1
AJ

```

```output1
81

```






```input2
1?AA

```

```output2
100

```



