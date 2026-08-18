<h1>ExpNo 4 : Implement A* search algorithm for a Graph</h1> 
<h3>Name: K Mithran A</h3>
<h3>Register Number: 212225220064 </h3>
<H3>Aim:</H3>
<p>To ImplementA * Search algorithm for a Graph using Python 3.</p>
<H3>Algorithm:</H3>


A* Search Algorithm
<ol>
<li> Initialize the open list</li>
<li> Initialize the closed list put the starting node on the open list (you can leave its f at zero)</li>
<li> While the open list is not empty<br>
    a. Find the node with the least f on 
       the open list, call it "q"<br>
    b. Pop q off the open list<br>
    c. Generate q's 8 successors and set their parents to q for each successor<br><ol>
        i. If successor is the goal, stop search<br>
        ii. Else, compute both g and h for successor
          <br>
          successor.g = q.g + distance between successor and successor.h = distance from goal to 
          successor (This can be done using many 
          ways, we will discuss three heuristics- 
          Manhattan, Diagonal and Euclidean 
          Heuristics)<br>
          successor.f = successor.g + successor.h<br>
        iii. if a node with the same position as successor is in the OPEN list which has a lower f than successor, skip this successor <br>
        iv. if a node with the same position as 
            successor  is in the CLOSED list which has
            a lower f than successor, skip this successor
            otherwise, add  the node to the open list
     end (for loop)<br></ol>
