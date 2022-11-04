---
title: "Structure-Aware Antibiotic Resistance Classification
using Graph Neural Networks"
collection: publications
permalink: /publication/arg
excerpt: "We propose a novel deep learning model to classify Antibiotic Resistance using protein sequence and structure [Read More](https://aymenqabel.github.io/publication/arg)"
date: '2022-10-03'
venue: 'Accepted at AI4Science at Neurips 2022'
video : 
code: 
paperurl: https://www.biorxiv.org/content/10.1101/2022.10.06.511103v1
citation: '<strong>Aymen Qabel</strong>, Michalis Vazirgiannis'
abstract: "Antibiotics are traditionally used to treat bacterial infections. However, bacteria can develop immunity to drugs, making them ineffective and thus posing a serious threat to global health. Identifying and classifying the genes responsible for this resistance is critical for the prevention, diagnosis, and treatment of infections as well as the understanding of its mechanisms. Previous methods developed for this purpose have mostly been sequence-based, relying on comparison to existing databases or machine learning models trained on sequence features. However, genes with comparable functions may not always have similar sequences. As a result, in this paper, we develop a deep learning model that uses the protein structure as a complement to the sequence to classify novel ARGs (antibiotic resistant genes), which we expect to provide more useful information than the sequence alone. The proposed approach consists of two steps. First, we capitalize on the celebrated AlphaFold model to predict the 3D structure of a protein from its amino acid sequence. Then, we process the sequence using a transformers-based language model while we also apply a graph neural network to the graph extracted from the structure. We evaluate the proposed architecture on a standard benchmark dataset where it outperforms state-of-the-art methods.
"
# figure_1: "goat_venn.jpg"
# caption_1: "An illustration of the Partial Information Decomposition for the case of one central node and two neighbors. The blue and the red circle represent the mutual information provided by the two neighbors about the central node. Each of these mutual information terms contains two atomic parts: $I(u:v_1)$ consists of the unique information in the $v_1$ neighbor $(U_{v_1}$, blue patch) and the information shared with $v_2$ neighbor ($R$, purple patch). Similarly, $I(u:v_2)$ consists of the unique information in $v_2$ neighbor ($U_{v_2}$, red patch) and again the shared information $R$.  The joint mutual information $I(u : v_1,v_2)$ is represented by the yellow box encompassing the inner two circles. $I(u : v_1,v_2)$ consists of four elements: the unique information in $v_1$ neighbor, the unique information in $v_2$ neighbor, the redundant information among the two neighbors and additionally the synergistic information, $I(u : v_1,v_2) = U_{v_1} + U_{v_2} + R + S $" 
# width_1: 450
# figure_2: "goat_model.jpg"
# caption_2: "An illustration of the aggregation and update of the representation of node $v_i$ using a GOAT layer.<br> A self-attention mechanism is used in order to obtain a ranking between the nodes of the neighborhood and then the ordered neighborhood is given as input into a sequence model (LSTM) to produce the updated representation of node $v_i$."
# width_2 : 1000
---
