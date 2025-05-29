<p align="justify">Products of a factory are packed into cylindrical boxes. All boxes have the same bases. A height of a box is a non-negative integer being a power of 2, i.e. it is equal to 2<i><sup>i</sup></i> for some <i>i</i> = 0, 1, 2, ... . The number <i>i</i> (exponent) is called a size of a box. All boxes contain the same goods but their value may be different. Goods produced earlier are cheaper. The management decided, that the oldest (cheapest) goods should be sold out first. From the warehouse goods are transported in containers. Containers are also cylindrical. A diameter of each container is a little bigger than a diameter of a box, so that boxes can be easily put into containers. A height of a container is a non-negative power of 2. This number is called a size of a container. For safe transport containers should be tightly packed with boxes, i.e. the sum of heights of boxes placed in a container have to be equal to the height of this container. A set of containers was delivered to the warehouse. Check if it is possible to pack all the containers tight with boxes that are currently stored in the warehouse. If so, find the minimal value of goods that can be tightly packed into these containers. </p>

<p align="justify">Consider a warehouse with 5 boxes. Their sizes and values of their contents are given below: </p>
<pre>1 3
1 2
3 5
2 1
1 4
</pre>
<p align="justify">Two containers of size 1 and 2 can be tightly packed with two boxes of total value 3, 4 or 5, or three boxes with total value 9. The container of size 5 cannot be tightly packed with boxes from the warehouse. </p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads descriptions of boxes (size, value) from a warehouse and descriptions of containers (how many containers of a given size we have); </li>
        <li align="justify">checks if all containers can be tightly packed with boxes from the warehouse and if so, computes the minimal value of goods that can be tightly packed into these containers; </li>
        <li align="justify">writes the result. </li>
</ul></div>

<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of a test case there is an integer <i>n</i>, 1 &lt;= <i>n</i> &lt;= 10000, which is the number of boxes in the warehouse. In each of the following <i>n</i> lines there are written two non-negative integers separated by a single space. These numbers describe a single box. First of them is the size of the box and the second - the value of goods contained in this box. The size is not greater than 1000 and the value is not greater than 10000. The next line contains a positive integer <i>q</i>, which is the number of different sizes of containers delivered to the warehouse. In each of the following <i>q</i> lines there are two positive integers separated by a single space. The first integer is the size of a container and the second one is the number of containers of this size. The maximal number of containers is 5000, a size of a container is not greater than 1000. </p>

<h3>Output</h3>
<p align="justify">For each test case your program should output exactly one line containing:</p>
<div align="justify"><ul>
        <li align="justify">a single word "No" if it is not possible to pack the containers from the given set tight with the boxes from the warehouse, or </li>
        <li align="justify">a single integer equal to the minimal value of goods in boxes with which all the containers from the given set can be packed tight. </li>
</ul></div>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
5
1 3
1 2
3 5
2 1
1 4
2
1 1
2 1

<b><tt>Sample output:</tt></b>
3
</pre>