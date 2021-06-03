# comp305-group16-project
COMP305 Term Project

Meeting #1:

Completed Steps

- The implementations of the graphs are discussed (Adjacency list, adjacency map, matrix..) and decided to use adjacency list to solve our problem.
- One solution found which includes transposing the graph and running Dijkstra's algorithm.
- The correctness is discussed and it was decided to use BFS algorithm to find all reachable nodes.

TO DO 
- Think about the implementation of the algorithm and graph implementation.

Meeting #2:

Completed Steps

- The implementation of BFS algorithm is done. 
- For the correctness, after transposing the graph, BFS algorithm is executed for all nodes with given ticket credit.
- Time complexity is O(V*E + E^2) and space complexity O(V^2)

TO DO 

- Are there another solutions and to the problem.
- If we use adjacency map, will there be any upgrade on the space complexity.
- Can we do recursive?
- Object-oriented solutions?

Meeting #3

Completed Steps

- Recursive DFS algorithm implemented to solve the question.
- Although the time complexity is O(V*E + E^2) again in this algortihm, the overall performance of the DFS was better.
- No need to use adjacency map.

TO DO  

- Search for another solution.
- Think about the I/O integration.

Meeting #4

Completed Steps

- Another solution is found which based on the idea that we are starting to traverse from one node. When we reach a node we increase the accessibility of this reached node by one. 
- This solution is more efficient compared the previous ones because the time complexity is O(t*N) where t is credit of the ticket and N is the number of vertices in the graph.


TO DO

- Is this solution can be upgraded? (for example using dynmamic programming or other recursive methods)
- The I/O integration will be different because this time no need to transpose the graph.


Meeting #5

Completed Steps

- I/O integration is done.
- No need to new solution because this is good enough.
- Complexity and time that the algorithm consumed is found for different test cases.

TO DO

- Create slides 




HOW TO RUN

The jupyter notebook file has different versions of the code from base to final. The executed version will be version 4. Because it has the all stuff from I/O integration to printing the results. You can use Shift + Enter.


TEST CASES

Gezgin test-case 1 results: [1, 2, 4, 5, 3, 1] (correct)
Gezgin test-case 2 results: [3, 3, 3, 2, 2] (correct
Gezgin test-case 3 and 4 results: these are big data and can be obtained from code. (correct also)


Gezgin test-case 3 and 4 : 6 minutes for case 3 and aproximately 1 hour for case 4.

FINAL ALGORITHM 

It is based on the straight forward traversing and updating efficiently.

We are start to traverse from node 1 and we are try to reach as far as from this node depending on the credit that we have. While we are traversing, we are updating of reachability counter of the visited nodes by one each time. When we check all the reachability condition for all nodes, we are returning the number of visits for all nodes.
And the time complexity is O(t*N)
 




























