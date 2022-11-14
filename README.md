USING FLOYD - WARSHALL ALGORITH To iterate over all my vertices to first find which ones were odd
I did  currentVertex->nonVirtualDegrees % 2 == 1 ) non virtual degrees helped me distiguinsh between which edges
were inserted initally when I read from the text file and which ones were from when I filled in virtual 
edges such as if it were mirror vertexes like (1,1) then I would set the weight to 0
but if the edges were anything else and they weren't already inserted then I would set the new edge to "virtual" from 
"non-virtual" then I would set the weight of that edge of a very large number, could't use infinity because when doing the comparison for FloydWarshall when you 
add it would go past the largest int allowed which in turn would be negative.

FLYOD-WARSHALL ALGO = O(n^3)
I used 3 for loops
SUDO CODE:
        
for  k =1 to n do

    for i = 1 to n do

        for j =1 to n do

        if(lovateEdge(i,j)) > (locateEdge(i,k) + locateEdge(k,j))
        updateWeighti,j,locateEdgeWeight);



Side notes:

initialize all weights from given graph to be 1 
then reinsert the 'missing edges' to either 0 or pos infinity 


CONTAINS DFS / DFS-VISIT / FLOYD-WARSHALL / FLOYD-WARSHALL-ODD 
