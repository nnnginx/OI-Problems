<p>Jai and Gopi are best friends. Both of them have a lot of girlfriends although they are nerds!!! One day one of gopi��s girlfriends came to him and asked him to prove his love for her. Unfortunately Gopi has a meeting with another girlfriend and asks his best friend Jai to help him. Jai with an idea of increasing his girlfriends count accepts immediately. Jai on hearing the task finds it so simple and so asks his junior to complete the task which is you.</p>
<p>&nbsp;</p>
<p>You are given a room of length <strong>L</strong> and breadth <strong>B</strong> which is dividen into unit cells. In each unit cell there are some gems which amount to a certain value which can be positive, negative or even zero. You are asked to answer <strong>T</strong> queries. Each query consists of a number <strong>N</strong> and you need to collect gems from <strong>N </strong>unit cells such that the value of <strong>N</strong> unit cells when summed up must be maximum. The selection of <strong>N </strong>unit cells in a room of length L and breadth B must be in such a way that it must be a small room of length say some <strong>x</strong> and breadth some <strong>y</strong> provided <strong>x*y=N</strong>.If No such value for x and y exist then print -1.</p>
<p>&nbsp;</p>
<p><strong>Input</strong></p>
<p>First line of input contains two space separated integers L and B which denotes the length and breadth of the room.</p>
<p>Following L lines contains B elements in each line each element specifying the value of the gems.</p>
<p>Next line contains T which is the number of queries.</p>
<p>Following T lines contains T elements where each element is the number N.</p>
<p><strong>1&lt;=L,B&lt;=1000</strong></p>
<p>All the L*B elements(x) will be in the range <strong>-100&lt;=x&lt;=100</strong></p>
<p><strong>1&lt;=T&lt;=10</strong></p>
<p><strong>1&lt;=N&lt;=10000</strong></p>
<p><strong>Output</strong></p>
<p>Print the maximum value that can be obtained for each value of N.</p>
<p><strong>Sample case</strong></p>
<p><strong>Input</strong></p>
<p>3 4</p>
<p>1 -2 3 -4</p>
<p>-5 6 -7 8</p>
<p>9 -10 11 -12</p>
<p>3</p>
<p>1</p>
<p>5</p>
<p>6</p>
<p><strong>Output</strong></p>
<p>11</p>
<p>-1</p>
<p>4</p>