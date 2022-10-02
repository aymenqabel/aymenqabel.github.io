---
title: "K-memBERT estimates cancer prognosis upon consultation"
collection: publications
permalink: /publication/kmembert
excerpt: "We propose a transformer-based model for survival prediction. [Read More](https://aymenqabel.github.io/publication/arg)"
date: '2022-10-03'
venue: 'Preprint'
video : 
code: 
paperurl: 
citation: '<strong>Aymen Qabel</strong>, Loic Verlingue'
abstract: "Prognosis estimation is one of the major components to take into account to guide therapeutic strategy of patients with cancer. Various data types have been used for prognostic estimation of patients affected by cancer but clinical documents have been under evaluated for this task, although it is the basic working material for physicians.

We fine-tuned and adapted CamemBERT, a French Transformer (a type of deep learning model for free text data), to predict the time to death of patients from Gustave Roussy Cancer Center (GR). Training, validation and test sets followed an 88-02-10 random split rule on individual patients. We introduced three different workflows evaluated on the validation set: (1) K-memBERT-base that takes one single document as input, (2) K-memBERT-conflation that aggregates multiple K-memBERT-base predictions with conflation, and (3) K-memBERT-T2 that stacks two transformers architecture to input a sequence of medical reports. CamemBERT-base and a Random Forest model were used as control. We then externally tested the performance of the best model on a cohort of patients of the Centre Léon Bérard (CLB). 

We used 2.9 million documents corresponding to 36124 patients in the GR cohort and 143k documents corresponding to 17633 patients in the CLB cohort. K-memBERT-T2 outperformed the other models and reached a Pearson correlation of 0.655 between the true and predicted survival on the GR test cohort and of 0.622 for the CLB external test cohort. The binary survival prediction AUC at 3 months was 0.852, at 1 year 0.817, and at mean survival (701 days) 0.827 for the GR test cohort and 0.875, 0.806 and 0.789 for the CLB cohort. K-memBERT-T2 had better prognostic performance than the performance status of patients, independently of this information. The errors were tempered by concomitant low confidence predictions, and K-memBERT-T2 comes with the interpretation of medical words importance on patients predicted survival.

K-memBERT-T2 generalized well across cohorts and french institutions and has competitive prognostic performances compared to models using other input data types, routine scores and cancer specialists, with the fastest and easiest implementation overall.
"
# figure_1: "goat_venn.jpg"
# caption_1: "An illustration of the Partial Information Decomposition for the case of one central node and two neighbors. The blue and the red circle represent the mutual information provided by the two neighbors about the central node. Each of these mutual information terms contains two atomic parts: $I(u:v_1)$ consists of the unique information in the $v_1$ neighbor $(U_{v_1}$, blue patch) and the information shared with $v_2$ neighbor ($R$, purple patch). Similarly, $I(u:v_2)$ consists of the unique information in $v_2$ neighbor ($U_{v_2}$, red patch) and again the shared information $R$.  The joint mutual information $I(u : v_1,v_2)$ is represented by the yellow box encompassing the inner two circles. $I(u : v_1,v_2)$ consists of four elements: the unique information in $v_1$ neighbor, the unique information in $v_2$ neighbor, the redundant information among the two neighbors and additionally the synergistic information, $I(u : v_1,v_2) = U_{v_1} + U_{v_2} + R + S $" 
# width_1: 450
# figure_2: "goat_model.jpg"
# caption_2: "An illustration of the aggregation and update of the representation of node $v_i$ using a GOAT layer.<br> A self-attention mechanism is used in order to obtain a ranking between the nodes of the neighborhood and then the ordered neighborhood is given as input into a sequence model (LSTM) to produce the updated representation of node $v_i$."
# width_2 : 1000
---
