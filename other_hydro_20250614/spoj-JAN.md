<p><em>Original problem statement (in Polish) can be found <a href="https://pizza.natodia.net/static/tasks/2017/eliminations/jasnowidz.pdf">here</a>.</em></p>

<p>The annual Congress of Mages is approaching. Januarius the Clairvoyant intends to participate in it. He has to somehow reach the city where the convention takes place.</p>

<p>His favourite means of transportation is railway. He plans to travel using a convenient, direct connection. The train will visit <strong>n</strong> stations, numbered with consecutive integers. It will depart from station number 1, with station number <strong>n</strong> as its destination. Remaining stations are intermediate - the train will visit them in order, according to their numbers.</p>

<p>Januarius likes travelling by train for a lot of reasons - it's comfortable, you can admire the landscape in peace - but most importantly, tickets are quite cheap. National Railways determined that cost of the trip depends only on the number of sections between stations covered during the ride. Ticket for <strong>i</strong> sections costs <strong>w<sub>i</sub></strong>. Obviously, the prices become higher when the trip gets longer.</p>

<p>You could also travel without a ticket if you're feeling adventurous, but of course there is a risk of unexpected ticket inspection, which can happen during the ride between two consecutive stations. Life of the clairvoyant is devoid of any surprises though - Januarius knows exactly when there will be an inspection. He doesn't have to buy full ticket - it's only important to have valid ticket during the inspection (starting station can be any station before the inspection, and the destination can be any station after the inspection).</p>

<p>There are two ways to buy a ticket - from the ticket office at the station, or already on the train, from the ticket inspector. There are limitations though. If you board the train without a ticket, you have to find the inspector immediately after the departure. He only sells tickets starting from the station you boarded the train at. Also, if you boarded the train at the station with a ticket office, you have to pay an additional constant fee of <strong>d</strong>.</p>

<p>Januarius has no time to get off the train during the ride, so he can either buy the ticket at the first station in a ticket office, or at any station from the inspector (he can approach him immediately after the departure from the station and tell him he just boarded the train). </p>

<p>Find the cheapest ticket-buying strategy. You must have a valid ticket during every inspection.</p>

<h3>Input</h3>
<p>The first line contains a single integer <strong>t</strong>, denoting the number of testcases. Then, descriptions of the testcases follow.</p>
<p>First line of the description consists of three integers <strong>n</strong>, <strong>k</strong> and <strong>d</strong> - number of stations, number of inspections and an additional fee for buying a ticket from the inspector in case there is a ticket office at the station (1 &lt;= <strong>n</strong> &lt;= 10<sup>6</sup>, 1 &lt;= <strong>k</strong> &lt;= 1000, 1 &lt;= <strong>d</strong> &lt;= 10<sup>9</sup>).</p>
<p>In the second line there is a string of length <strong>n</strong>. If station number <strong>i</strong> has a ticket office, <strong>i</strong>-th character of this string is "1", otherwise it's "0". </p>
<p>In the third line there are <strong>n</strong>-1 integers. <strong>i</strong>-th number <strong>w<sub>i</sub></strong> denotes price of covering <strong>i</strong> sections. (1 &lt;= <strong>w<sub>i</sub></strong> &lt;= 10<sup>9</sup>, <strong>w<sub>i</sub></strong> &lt; <strong>w<sub>i+1</sub></strong>).</p>
<p>In the last line there are <strong>k</strong> integers <strong>s<sub>i</sub></strong> - stations numbers. <strong>i</strong>-th ticket inspection will take place between the station number <strong>s<sub>i</sub></strong> and the station number <strong>s<sub>i</sub></strong>+1. (1 &lt;= <strong>s<sub>i</sub></strong> &lt;= <strong>n</strong>-1, <strong>s<sub>i</sub></strong> &lt; <strong>s<sub>i+1</sub></strong>)</p>

<h3>Output</h3>
<p>For every testcase you should output a ticket-buying strategy that minimizes total cost. Description of the strategy starts with two integers <strong>s</strong> and <strong>b</strong> - total cost of the tickets and number of tickets (1 &lt;= <strong>b</strong> &lt;= <strong>n</strong>). Descriptions of the tickets should follow. One ticket description consists of two integers <strong>p<sub>i</sub></strong> and <strong>c<sub>i</sub></strong> - starting station and number of segments for which the ticket is valid. (1 &lt;= <strong>p<sub>i</sub></strong> &lt; <strong>n</strong>, 1 &lt;= <strong>c<sub>i</sub></strong> &lt;= <strong>n</strong>-<strong>p<sub>i</sub></strong>).</p>
<p>You should describe <strong>b</strong> tickets, their total cost must be equal to <strong>s</strong>, and it has to be minimal.</p>

<h3>Example</h3>
<p>Input:</p>
<pre>1
5 2 5
11001
2 6 7 10
2 4</pre>
<p>Output:</p>
<pre>8 2
1 2
4 1</pre>

<h3>Explanation</h3>
<p>There are two inspections - between stations 2 and 3, and between stations 4 and 5. Januarius can buy a ticket in the ticket office from the station number 1 to the station number 3, and another one from the inspector from station number 4 to station number 5, and it will cost him 6+2=8.</p>
<p>If he bought the first ticket from the second station instead from the first, it would be more expensive - there is a ticket office at the second station, so there will be an additional fee for buying the ticket from the inspector. (2+5+2=9).</p>