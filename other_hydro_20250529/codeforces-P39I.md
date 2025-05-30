## Description

<div><p>In a Berland city S*** there is a tram engine house and only one tram. Three people work in the house — the tram driver, the conductor and the head of the engine house. The tram used to leave the engine house every morning and drove along his loop route. The tram needed exactly <span class="tex-span"><i>c</i></span> minutes to complete the route. The head of the engine house controlled the tram’s movement, going outside every <span class="tex-span"><i>c</i></span> minutes when the tram drove by the engine house, and the head left the driver without a bonus if he was even one second late.</p><p>It used to be so. Afterwards the Berland Federal Budget gave money to make more tramlines in S***, and, as it sometimes happens, the means were used as it was planned. The tramlines were rebuilt and as a result they turned into a huge network. The previous loop route may have been destroyed. S*** has <span class="tex-span"><i>n</i></span> crossroads and now <span class="tex-span"><i>m</i></span> tramlines that links the pairs of crossroads. The traffic in Berland is one way so the tram can move along each tramline only in one direction. There may be several tramlines between two crossroads, which go same way or opposite ways. Every tramline links two different crossroads and for each crossroad there is at least one outgoing tramline.</p><p>So, the tramlines were built but for some reason nobody gave a thought to increasing the number of trams in S***! The tram continued to ride alone but now the driver had an excellent opportunity to get rid of the unending control of the engine house head. For now due to the tramline network he could choose the route freely! Now at every crossroad the driver can arbitrarily choose the way he can go. The tram may even go to the parts of S*** from where it cannot return due to one way traffic. The driver is not afraid of the challenge: at night, when the city is asleep, he can return to the engine house safely, driving along the tramlines in the opposite direction.</p><p>The city people were rejoicing for some of the had been waiting for the tram to appear on their streets for several years. However, the driver’s behavior enraged the engine house head. Now he tries to carry out an insidious plan of installing cameras to look after the rebellious tram.</p><p>The plan goes as follows. The head of the engine house wants to install cameras at some crossroads, to choose a period of time <span class="tex-span"><i>t</i></span> and every <span class="tex-span"><i>t</i></span> minutes turn away from the favourite TV show to check where the tram is. Also the head of the engine house wants at all moments of time, divisible by <span class="tex-span"><i>t</i></span>, and only at such moments the tram to appear on a crossroad under a camera. There must be a camera on the crossroad by the engine house to prevent possible terrorist attacks on the engine house head. Among all the possible plans the engine house head chooses the plan with the largest possible value of <span class="tex-span"><i>t</i></span> (as he hates being distracted from his favourite TV show but he has to). If such a plan is not unique, pick the plan that requires the minimal possible number of cameras. Find such a plan.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of crossroads and tramlines in S*** respectively. The next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the tramlines in "<span class="tex-span"><i>u</i></span> <span class="tex-span"><i>v</i></span>" format, where <span class="tex-span"><i>u</i></span> is the initial tramline crossroad and <span class="tex-span"><i>v</i></span> is its final crossroad. The crossroads are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the engine house is at the crossroad number <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>In the first line output the value of <span class="tex-span"><i>t</i></span>. In the next line output the value of <span class="tex-span"><i>k</i></span> — the required number of the cameras. In the next line output space-separated numbers of the crossroads, where the cameras should be installed. Output the numbers in increasing order.</p></div>


## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of crossroads and tramlines in S*** respectively. The next <span class="tex-span"><i>m</i></span> lines contain the descriptions of the tramlines in "<span class="tex-span"><i>u</i></span> <span class="tex-span"><i>v</i></span>" format, where <span class="tex-span"><i>u</i></span> is the initial tramline crossroad and <span class="tex-span"><i>v</i></span> is its final crossroad. The crossroads are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and the engine house is at the crossroad number <span class="tex-span">1</span>.</p>


## Output

<p>In the first line output the value of <span class="tex-span"><i>t</i></span>. In the next line output the value of <span class="tex-span"><i>k</i></span> — the required number of the cameras. In the next line output space-separated numbers of the crossroads, where the cameras should be installed. Output the numbers in increasing order.</p>


## Samples

```input1
4 5
1 2
2 3
3 4
4 1
1 4

```

```output1
2
2
1 3

```



