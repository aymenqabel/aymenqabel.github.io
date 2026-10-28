---
title: "ConforNets: Latents-Based Conformational Control in OpenFold3"
collection: publications
short: "ConforNets"
permalink: /publication/confornets
excerpt: "We introduce ConforNets, channel-wise affine transforms of OpenFold3's pair latents that steer predictions toward alternative protein conformations. [Read More](https://aymenqabel.github.io/publication/confornets)"
date: '2026-04-20'
venue: 'Preprint'
video : 
code: https://github.com/aqlaboratory/confornets
paperurl: https://arxiv.org/abs/2604.18559
citation: 'Minji Lee, Colin Kalicki, Minkyu Jeon, <strong>Aymen Qabel</strong>, Alisia Fadini, Mohammed AlQuraishi'
abstract: "Models of the AlphaFold family usually predict a single dominant conformation, even for proteins with biologically relevant alternative states. We study where and how to perturb the latent representations of AlphaFold3-style architectures to recover these states, and introduce ConforNets: channel-wise affine transforms applied to the pre-Pairformer pair latents of OpenFold3. Because they act globally rather than residue by residue, ConforNets can be reused across proteins. They achieve state-of-the-art results on multi-state benchmarks of diverse conformational changes, and a ConforNet trained on one protein can transfer a conserved conformational change to other members of its family."
---
