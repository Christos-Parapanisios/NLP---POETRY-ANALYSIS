In this notebook i wanted to demonstrate the process of analyzing semantic relationships between phrases using a graph-based approach. The phrases are taken from a poem.

Phrase Embedding and Similarity Calculation
Using a pre-trained Sentence-BERT (SBERT) model, the phrases are transformed into embeddings—numerical vectors that capture their semantic meaning. Cosine similarity is then used to measure the degree of similarity between each pair of phrases. This allows for quantifying how closely the phrases are related in meaning.

Graph Construction
Two types of graphs are built:

An unweighted graph for computing centrality measures based on simple connections between phrases. A weighted graph where the edge weights represent the cosine similarity between the phrases, capturing the strength of their semantic connections.

Centrality and Semantic Strength Analysis
Centrality measures such as degree, betweenness, closeness, and eigenvector centrality are calculated on the unweighted graph to identify the most influential phrases. The weighted graph is used to compute each phrase’s total semantic strength by summing the edge weights, allowing for an analysis of how central or isolated a phrase is in terms of meaning.

Visualization
The notebook includes a visualization of the semantic graph, with nodes colored to represent their semantic strength, offering an intuitive way to observe the relationships between phrases.
