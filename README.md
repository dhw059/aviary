# Sampnn
Structure Agnostic Message Passing Neural Network

## Premise
In materials discovery applications often we know the composition of trial materials but have little knowledge about the structure.

Most current SOTA results within the field of machine learning for materials discovery are reliant on already knowing the structure of the material. Whilst this can be helpful for interpolating within given systems it means that out ML applications must be intrinsically  dependant on costly DFT calculations to first find structures fro trial compositions. Whilst this would not be prohibitive it adds an additional level of complexity.

In a similar vein to other materials agnostic platforms (i.e. [MAGPIE](http://oqmd.org/static/analytics/magpie/doc/)) the aim of this model is to be able to determine properties (to reasonable accuracy) based solely on the composition of a material.

## Message Passing Neural Networks
Recent progress in the study of small molecules has built upon the use of message passing neural networks. The structure of the graphs can be described by an adjacency matrix and the nodes contain relevant atomic features. Similar attempts are already progressing in application of such networks to extended periodic crystals although notable issues exist in how to represent dopants in such graphs and how much of the structure we can take as prior knowledge. This work is motivated by a case study on High Temperature Superconductors where the role of dopants is critical therefore here we hope to develop a structure agnostic approach that therefore enables dopants to be handled trivially.

### TODO:
* Include the stiochiometric weights in the message function
* Update via hebbian type algorithm to strengthen anion-cation type weights and weaken anion-anion and cation-cation weights.

## Acknowledgements

If you use this code please cite our work for which this model was built:

[Structure Agnostic Message Passing Neural Networks (placeholder)](http://www.tcm.phy.cam.ac.uk/profiles/reag2/)

please also consider citing the following paper whose CGCNN framework we took as a starting point for developing Sampnn:

[Crystal Graph Convolutional Neural Networks for an Accurate and Interpretable Prediction of Material Properties](https://link.aps.org/doi/10.1103/PhysRevLett.120.145301)

## Disclaimer
This in research code and it is shared without support or any guarentee on its quality. However, if you do find an error please submit a pull request or raise an issue and I will try my best to solve it.