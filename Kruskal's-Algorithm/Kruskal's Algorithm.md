## What is a Spanning Tree?
A Spanning tree is a subset to a connected graph G, where all the edges are connected, i.e, one can traverse to any edge from a particular edge with or without intermediates. Also, a spanning tree must not have any cycle in it. Thus we can say that if there are N vertices in a connected graph then the no. of edges that a spanning tree may have is N-1.

## What is a Minimum Spanning Tree? 
Given a connected and undirected graph, a spanning tree of that graph is a subgraph that is a tree and connects all the vertices together. A single graph can have many different spanning trees. A minimum spanning tree (MST) or minimum weight spanning tree for a weighted, connected, undirected graph is a spanning tree with a weight less than or equal to the weight of every other spanning tree. The weight of a spanning tree is the sum of weights given to each edge of the spanning tree.

## How many edges does a minimum spanning tree has? 
A minimum spanning tree has (V – 1) edges where V is the number of vertices in the given graph. 

## How to find MST using Kruskal’s algorithm?
1.Sort all the edges in non-decreasing order of their weight. 

2.Pick the smallest edge. Check if it forms a cycle with the spanning tree formed so far. If cycle is not formed, include this edge. Else, discard it. 

3.Repeat step#2 until there are (V-1) edges in the spanning tree.

## Illustration:
### Input Graph:

![image](https://user-images.githubusercontent.com/100795596/206441931-977e2862-24c8-4996-9a6c-71da8182030c.png)

The graph contains 9 vertices and 14 edges. So, the minimum spanning tree formed will be having (9 – 1) = 8 edges. 

After sorting:
Weight   Src    Dest
1         7      6
2         8      2
2         6      5
4         0      1
4         2      5
6         8      6
7         2      3
7         7      8
8         0      7
8         1      2
9         3      4
10        5      4
11        1      7
14        3      5

Now pick all edges one by one from the sorted list of edges.

#### Step 1:
Pick edge 7-6: No cycle is formed, include it. 

![image](https://user-images.githubusercontent.com/100795596/206442205-906793e3-51dd-4102-9c31-8be67e6438d9.png)

#### Step 2:
Pick edge 8-2: No cycle is formed, include it. 

![image](https://user-images.githubusercontent.com/100795596/206442309-7d1cbe94-64ae-4286-b3ed-83d990f25365.png)

#### Step 3:
Pick edge 6-5: No cycle is formed, include it. 

![image](https://user-images.githubusercontent.com/100795596/206442419-6f53399c-7c37-4ca6-bb35-57c4c8016320.png)

#### Step 4: 
Pick edge 0-1: No cycle is formed, include it. 

![image](https://user-images.githubusercontent.com/100795596/206442506-b33a4caa-d11a-45e6-b78c-61404bbb69d3.png)

#### Step 5: 
Pick edge 2-5: No cycle is formed, include it. 

![image](https://user-images.githubusercontent.com/100795596/206442621-9b025a99-6b22-4f2d-911a-e17d3522db1a.png)

#### Step 6: 
Pick edge 8-6: Since including this edge results in the cycle, discard it.

#### Step 7: 
Pick edge 2-3: No cycle is formed, include it. 

![image](https://user-images.githubusercontent.com/100795596/206442769-9f0da988-5a67-448a-9f0a-d6bed19e2153.png)

#### Step 8: 
Pick edge 7-8: Since including this edge results in the cycle, discard it.

#### Step 9: 
Pick edge 0-7: No cycle is formed, include it. 

![image](https://user-images.githubusercontent.com/100795596/206442975-fece9f7c-1ec1-4aed-a9be-634b93959839.png)

#### Step 10:  
Pick edge 1-2: Since including this edge results in the cycle, discard it.

#### Step 11: 
Pick edge 3-4: No cycle is formed, include it. 

![image](https://user-images.githubusercontent.com/100795596/206443172-9ab74a0b-dff8-4e13-ad40-44ffafdd7f31.png)

### Note: 
Since the number of edges included in the MST equals to (V – 1), so the algorithm stops here.
