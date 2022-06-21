---
title: "Graph-based Neural Architecture Search with Operation Embeddings"
collection: publications
permalink: /publication/operation_embeddings_for_nas
excerpt: " We propose the replacement of fixed operator encoding with learnable representations in the optimization process. [Read More](https://michailchatzianastasis.github.io/publication/operation_embeddings_for_nas) "
date: '2021-05-11'
venue: '<a href="https://neural-architecture-ppf.github.io/"> ICCV 2021 Workshop on Neural Architectures: Past, Present and Future </a>'
video : 'https://www.youtube.com/watch?v=-rZ4tpNvL6s'
code: 'https://github.com/MichailChatzianastasis/Graph-based_NAS_with_Operation_Embeddings'
paperurl: 'https://arxiv.org/pdf/2105.04885.pdf'
poster: 'https://github.com/MichailChatzianastasis/Graph-based_NAS_with_Operation_Embeddings/blob/master/Graph_based_neural_architecture_search_with_operation_embeddings_ICCV.pdf'
citation: '<strong>Michail Chatzianastasis</strong>, George Dasoulas, Georgios Siolas, Michalis Vazirgiannis'
abstract: " Neural Architecture Search (NAS) has recently gained
increased attention, as a class of approaches that automatically searches in an input space of network architectures. A
crucial part of the NAS pipeline is the encoding of the architecture that consists of the applied computational blocks,
namely the operations and the links between them. Most of
the existing approaches either fail to capture the structural
properties of the architectures or use a hand-engineered vector to encode the operator information. In this paper, we
propose the replacement of fixed operator encoding with
learnable representations in the optimization process. This
approach, which effectively captures the relations of different operations, leads to smoother and more accurate representations of the architectures and consequently to improved performance of the end task. Our extensive evaluation in ENAS benchmark demonstrates the effectiveness
of the proposed operation embeddings to the generation
of highly accurate models, achieving state-of-the-art performance. Finally, our method produces top-performing
architectures that share similar operation and graph patterns, highlighting a strong correlation between architecture’s structural properties and performance
"
figure_1: "nas_pipeline.jpg"
caption_1: "<strong>Workflow of Variational Graph Auto-Encoder for NAS with integration of Operation Embeddings</strong>. First, the corresponding directed acyclic graph $G_A=(A,\textbf{X})$ of the input architecture is constructed. Then, the operations $X$ are given as input in the operation embeddings layer, to obtain the embeddings $O(\textbf{X})$. Finally, the adjacency matrix and the operation embeddings are passed to the  auto-encoder." 
width_1: 750
---








