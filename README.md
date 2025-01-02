##Logical Zero Shot Learning

In real-life image recognition challenges, there are often too many object classes to get
labelled data for all possible classes. Moreover, there can be hierarchical semantic
relationships between the classes and it is impractical to train an image classication model
on each of the classes separately. Zero-shot learning aims to learn generalizable semantic
information from some classes during training, such that these semantics can be used to
identify unseen classes during inference. 


Existing works like An embarrassingly simple approach to zero-shot learning,
Romera-Paredes et al., 2015 (ESZSL) and Semantic Autoencoder for Zero-Shot Learning,
Kodirov et al.,2017 (SAE) learn a linear mapping from the visual features to the semantic
attribute space. SAE additionally uses a reconstruction error to train this mapping network.
During inference, attributes are obtained for the unseen classes using the mapping
network. The class with the closest attribute is the output.


The goal of this project is to explore if using neural networks instead of linear mappings
can improve this mapping function. Also, we use prior knowledge and logical
constraints to improve the attribute learning process.
