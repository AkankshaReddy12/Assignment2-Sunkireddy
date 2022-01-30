# Assignment2-Sunkireddy
# Aakanksha Reddy
###### Barbeque Nation

Barbeque Nation is loacted in Hyderabad.
It is a multi cuisine restraunt

Barbeque Nation is very famous for barbeque<br>
People can enjoy having food at Barbeque.

**northwest missouri state university**

---

# Route to Barbeque Nation
1. Take a public transport from airport.
2. Get down in Gachibowli.
9. Book a cab to Barbeque Nation.
---
#Food Menu

-Chicken
    
-Mutton

-Fish

**[Add](AboutMe.md)**

---


# Sports

This table is related to sports that has sports name,location and amount that shoud be paid<br>Sports are going to held in the locations mentioned

| Name   | location   | Amount |
|------- |------------|--------|
|Cricket |Hyderabad   |$100    |
|Badminton|Chennai    |$50     |
|Hockey   |Banglore   |$250    |
|Tennis   |Kolkata    |$36     |






# Next Heading

>The way to get started is to quit talking and begin doing.     -*Walt Disney*

>Life is what happens when you're busy making other plans.       -*John Lennon*

---

# Breadth-first Search

>Breadth-first search (BFS) is an algorithm for searching a tree data structure for a node that satisfies a given property. It starts at the tree root and explores all nodes at the present depth prior to moving on to the nodes at the next depth level. Extra memory, usually a queue, is needed to keep track of the child nodes that were encountered but not yet explored.
<https://en.wikipedia.org/wiki/Breadth-first_search>

```
vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}
```
<https://cp-algorithms.com/graph/breadth-first-search.html>

