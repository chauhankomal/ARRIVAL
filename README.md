# ARRIVAL

## Introduction

We introduce our method ARRIVAL, a random walks based algorithm to answer a traditional graph query: Reachability. We do this, keeping in mind that most networks today are labeled and reachability under certain constraints becomes an interesting problem. These queries nowadays are called Regular Path Queries. These queries are studied among many different semantics: existential, shortest and simple being the primary ones. We restrict ourselves to only Regualar Simple Paths, but our technique can easily be scaled to existential as well. We deal with all kinds of labels, be it on the node or edge or whether it be defined at the time of querying. We are also able to deal with large Dynamic Graphs with incoming flow of nodes, edges as well as labels.

## Running the Algorithm
To run the code, run "run.sh" with two arguments, 1: folder name of the dataset being used, 2: queryfilename inside folder 1,3: 1 if the graph is directed, 0 if undirected, 4: the maximum times that a node for which successor is not found, is searched

The folder should contain:
1. edgefile (edges.txt) (each line of the form u v l, where there is an edge from u to v with a label l, if l is not present it is assumed to be 1)
2. labelfile (labels.txt) (each line of the form u l, where node u has a label l, multiple labels on a node are allowed with newline) 
3. queryfile (query has to be of the form u v noderegex edgeregex, if no edgeregex is found it will be assumed to be (1)*).
