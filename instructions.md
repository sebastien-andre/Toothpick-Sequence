!(https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/0.png?raw=true)
<img src="images/0.png?" alt="Alt text" title="Optional title">

<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="https://tinman.cs.gsu.edu/~raj/my.css">
<title>CSc 1301 Honors Lab - Fall 2022</title>
</head>

<body style="background-color:#ADD8E6;">

<div id="page">
<div id="main-col">

<div class="section">
<h3>Programming Assignment 8 (Toothpick Sequence)</h3>
</div>

<div class="section">
<h4>Toothpick Sequence</h4>
In this programming assignment, you will develop a Python program to draw
the "Toothpick" sequence (<a href="https://en.wikipedia.org/wiki/Toothpick_sequence">Wikipedia</a>). You shall use the graphics.py package
from Zelle's textbook available at
<a href="https://mcsp.wartburg.edu/zelle/python/">Simple Graphics Library</a>
to solve this problem.
<P>The sequence begins with one toothpick (iteration 0) placed on a canvas vertically as shown below:

<P>
</P>

   ![i](https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/0.png "title")
<P>

   
<P>In subsequent iterations, new toothpicks are placed perpendicular to
open ends of previous toothpicks with the midpoint of the new toothpick placed
touching the open end.
Some toothpick arrangements, after 1, 2, 3, 4, and 8 iterations:
<P>
<img src="https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/1.png" width="100" height="100"/>
<img src="https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/2.png" width="100" height="100"/>
<img src="https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/3.png" width="100" height="100"/>
<img src="https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/4.png" width="100" height="100"/>
<img src="https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/8.png" width="100" height="100"/>
<P>Here are two more arrangements (after 24 and 32 iterations):
<P>
<img src="https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/24.png" width="400" height="400"/>
<img src="https://tinman.cs.gsu.edu/raj/1301/f22/p8-extracredit/32.png" width="400" height="400"/>
<P>The tricky part of the problem is to identify open ends that allow new
toothpicks to be placed at that end. It is not always that the two ends of
the new toothpick are open (sometimes they coincide with open end of another toothpick
at the end of an iteration), in which case we should not place the new toothpick
at such ends. The graphics.py package does not allow us to detect such coinciding
ends, however since the graphics window, GraphWin, is a sub-class of TKinter Canvas
class, we should be able to use some of the methods in the TKinter Canvas class to detect
such ends.
<P>The program should take the number of iterations as a command line input.
The program should pop open a Canvas Window and draw the toothpicks for the
number of iterations specified. It should then wait for a mouse click to terminate. 
It should also print to terminal the iteration #, #toothpicks added in each
iteration, as well as the total number of toothpicks added after each
iteration as shown in the output below.
<pre>
Mac-mini:p8-toothpick raj$ python3 Toothpick.py 8
Iteration#: 1 #Toothpicks added in this iteration: 2 Total #toothpicks= 3
Iteration#: 2 #Toothpicks added in this iteration: 4 Total #toothpicks= 7
Iteration#: 3 #Toothpicks added in this iteration: 4 Total #toothpicks= 11
Iteration#: 4 #Toothpicks added in this iteration: 4 Total #toothpicks= 15
Iteration#: 5 #Toothpicks added in this iteration: 8 Total #toothpicks= 23
Iteration#: 6 #Toothpicks added in this iteration: 12 Total #toothpicks= 35
Iteration#: 7 #Toothpicks added in this iteration: 8 Total #toothpicks= 43
Iteration#: 8 #Toothpicks added in this iteration: 4 Total #toothpicks= 47
Mac-mini:p8-toothpick raj$
</pre>
</div>


</div>
</div>
   
</body>
</html>


