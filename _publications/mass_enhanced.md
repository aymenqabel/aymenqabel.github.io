---
title: "Mass Enhanced Node Embeddings for Drug Repurposing"
collection: publications
permalink: /publication/mass_enhanced
excerpt: "We propose a node embedding algorithm for the problem of drug repurposing. The
proposed algorithm learns node representations that capture the
influence of nodes in the biological network by learning a mass term
for each node along with its embedding. [Read More](https://michailchatzianastasis.github.io/publication/mass_enhanced)"
date: '2022-06-10'
venue: ' <a href="https://icml-compbio.github.io">ICML 2022 Workshop on Computational Biology</a> and  <a href="https://hilab.di.ionio.gr/setn2022"> 12th EETN Conference on Artificial Intelligence (SETN 2022)</a> '

#video : 'https://www.youtube.com/watch?v=-rZ4tpNvL6s'
code: 'https://github.com/MichailChatzianastasis/Mass-Enhanced-Node-Embeddings-for-Drug-Repurposing'
paperurl: 'https://www.biorxiv.org/content/10.1101/2022.06.22.497214v1'
citation: '<strong>Michail Chatzianastasis</strong>, Giannis Nikolentzos, Michalis Vazirgiannis'
abstract: "Graph representation learning has recently emerged as a promising approach to solve pharmacological tasks by modeling biological networks.
Among the different tasks, drug repurposing, the task of identifying new uses for approved or investigational drugs, has attracted a lot of attention recently.
In this work, we propose a node embedding algorithm for the problem of drug repurposing.
The proposed algorithm learns node representations that capture the influence of nodes in the biological network by learning a mass term for each node along with its embedding.
We apply the proposed algorithm to a multiscale interactome network and embed its nodes (i.e. proteins, drugs, diseases and biological functions) into a low-dimensional space.
We evaluate the generated embeddings in the drug repurposing task.
Our experiments show that the proposed approach outperforms the baselines and offers an improvement of 53.33% in average precision over typical walk-based embedding approaches.
"
#figure_1: "goat_venn.jpg"
#caption_1: "An illustration of the Partial Information Decomposition for the case of one central node and two neighbors. The blue and the red circle represent the mutual information provided by the two neighbors about the central node. Each of these mutual information terms contains two atomic parts: $I(u:v_1)$ consists of the unique information in the $v_1$ neighbor $(U_{v_1}$, blue patch) and the information shared with $v_2$ neighbor ($R$, purple patch). Similarly, $I(u:v_2)$ consists of the unique information in $v_2$ neighbor ($U_{v_2}$, red patch) and again the shared information $R$.  The joint mutual information $I(u : v_1,v_2)$ is represented by the yellow box encompassing the inner two circles. $I(u : v_1,v_2)$ consists of four elements: the unique information in $v_1$ neighbor, the unique information in $v_2$ neighbor, the redundant information among the two neighbors and additionally the synergistic information, $I(u : v_1,v_2) = U_{v_1} + U_{v_2} + R + S $" 

#width_1: 450
#figure_2: "goat_model.jpg"
#caption_2: "An illustration of the aggregation and update of the representation of node $v_i$ using a GOAT layer.<br> A self-attention mechanism is used in order to obtain a ranking between the nodes of the neighborhood and then the ordered neighborhood is given as input into a sequence model (LSTM) to produce the updated representation of node $v_i$."
#width_2 : 1000
---
