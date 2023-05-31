# Community Detection Algorithm on Social Network

This repository contains an implementation of community detection algorithms, namely the Clique Percolation Method (CPM) and Girvan-Newman algorithm, applied on the polbooks.gml dataset. The goal is to identify communities within the social network represented by the dataset.

## Dataset

The polbooks.gml dataset is included in the repository. It represents a social network of political books, where each book is represented as a node and edges represent shared readership between books. The dataset is in GML (Graph Modeling Language) format, which is a textual representation of graph data.

## Algorithms

### Clique Percolation Method (CPM)

The Clique Percolation Method is a community detection algorithm based on finding overlapping cliques in a network. It works by first identifying all k-cliques in the graph and then merging the cliques that overlap in k-1 nodes. The resulting overlapping k-cliques form communities within the network.

### Girvan-Newman Algorithm

The Girvan-Newman algorithm is a hierarchical divisive algorithm that detects communities by iteratively removing edges with high betweenness centrality. It starts with the original network and calculates the betweenness centrality of all edges. The edge with the highest betweenness centrality is removed, and the process is repeated until no edges remain. The resulting disconnected components form the communities.
