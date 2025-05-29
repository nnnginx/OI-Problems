<p>A cellular provider has installed n towers to support their network. Each tower provides coverage in a 1km radius, and no two towers are closer than 1km to each other. The coverage region of this network is therefore the set of all points that are no more than 1km away from at least one tower. The provider wants as much of this region as possible to be connected, in the sense that a user at any point within a connected subregion can travel to any other point within the connected subregion without having to exit the subregion. Their current installation of towers may or may not already form a single connected region, but they have the resources to build one more tower wherever they want, including within 1km of an existing tower. Given that the provider is able to build one more tower, what is the maximum number of towers (including the new one) that can be included within a single connected subregion of coverage?</p>
<h3>Input</h3>
<p>Each input will consist of a single test case. Note that your program may be run multiple times on different inputs. The first line of input consists of a single integer n (1¡Ün¡Ü5,000) denoting the number of existing towers. Next follow n lines, each with 2 space separated floating-point numbers x and y (0¡Üx,y¡Ü100,000), denoting the location of a tower in km. It will be guaranteed that the optimal number of towers will not change even if the coverage radius of all the towers is increased or decreased by 10<sup>-6</sup> km.</p>
<h3>Output</h3>
<p>Ouput a single integer, denoting the maximum number of towers that can be within a single connected subregion of the network after installing one additional tower.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 <br>1.0 1.0 <br>3.1 1.0 <br>1.0 3.1 <br>3.1 3.1 <br>4.2 3.1

<strong>Output:</strong>
6</pre>