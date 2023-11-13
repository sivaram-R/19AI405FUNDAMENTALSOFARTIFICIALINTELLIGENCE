<h1>ExpNo 3 : Implement A* search algorithm for a Graph</h1> 
<h3>Name: JEEVAGOWTHAM S</h3>
<h3>Register Number: 212222230053</h3>
<H3>Aim:</H3>
<p>To ImplementA * Search algorithm for a Graph using Python 3.</p>
<H3>Algorithm:</H3>
// A* Search Algorithm
1.  Initialize the open list
2.  Initialize the closed list
    put the starting node on the open 
    list (you can leave its f at zero)

3.  while the open list is not empty
    a) find the node with the least f on 
       the open list, call it "q"

    b) pop q off the open list
  
    c) generate q's 8 successors and set their 
       parents to q
   
    d) for each successor
        i) if successor is the goal, stop search
        ```
        ii) else, compute both g and h for successor
          successor.g = q.g + distance between 
                              successor and q
          successor.h = distance from goal to 
          successor (This can be done using many 
          ways, we will discuss three heuristics- 
          Manhattan, Diagonal and Euclidean 
          Heuristics)
          
          successor.f = successor.g + successor.h

        iii) if a node with the same position as 
            successor is in the OPEN list which has a 
           lower f than successor, skip this successor

        iV) if a node with the same position as 
            successor  is in the CLOSED list which has
            a lower f than successor, skip this successor
            otherwise, add  the node to the open list
     end (for loop)
    ```  
    e) push q on the closed list
    end (while loop)
   
<hr>
<h2>Sample Graph I</h2>
<hr>

![image](https://github.com/Saibandhavi75/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/94208895/d4679838-4189-4a13-a0d0-f5e91867b064)

# Input & Output 1:
![image](https://github.com/Saibandhavi75/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/94208895/274755ef-4695-49e8-8cf1-1a0d28b8685b)


# Sample Graph II

![image](https://github.com/Saibandhavi75/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/94208895/e890b350-3953-4ec9-a938-241605e84bfe)

# Input & Output 2:
![image](https://github.com/Saibandhavi75/19AI405FUNDAMENTALSOFARTIFICIALINTELLIGENCE/assets/94208895/37b9fe97-9126-4a07-b370-1ae43cd6c4f6)

# Result;
Thus, a Graph was constructed, and the implementation of the A* algorithm for the same graph was executed successfully. The algorithm found the shortest path from the start node to the stop node, demonstrating its effectiveness in solving pathfinding problems.
