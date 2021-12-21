# SSLPA
#Semantic Speaker-Listener Label Propagation Algorithm \n
This repository contains supplementary material (code and data) for the paper: "Identifying specific semantic communities based on label propagation" 
The algorithm implementations require Python 3.x and the NetworkX library.
The main process of SSLPA
This paper proposes a community detection algorithm that combines network topology and textual node attributes to identify communities with specific 
semantic interpretations. We identify community structure while extracting communities’ topics rather than regarding them as two adjacent steps. 
This algorithm consists of four main stages. During initialization phase, the topological information and content of nodes are represented via 
two parallel and independent semantic label sets, then the labels are assigned TF-IDF extracted from node content as its initial weight. 
During the similarity measure phase, the semantic similarity between neighbor nodes is measured by the cosine of the angle between the vector 
representation of the corresponding labels. During the propagation phase, nodes choose labels from their neighbors according to the preference rules. 
A forgetting mechanism is adopted for filtering low frequency labels. In the final phase, nodes are divided into overlapping communities 
with certain coefficients once the stop criterion is met. 
## The code is still being improved, and the subsequent implementation process will be encapsulated to facilitate the implementation
