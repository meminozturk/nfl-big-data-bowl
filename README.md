# 13th place solution to NFL Big Data Bowl Competition in Kaggle

We developed a Deep Learning model consisting of Attention and Embedding layers on top of a Multilayer Perceptron.

Few words about how we came up with the model structure. To simplify we assume a rushing play consists of:

- A rusher, whose aim is to run forward as far as possible
- 11 defense players who are trying to stop the rusher
- 10 remaining offense players trying to prevent defenders from blocking or tackling the rusher

Embedding layers were used to represent player’s basic features (speed, direction and orientation) and their projections by other players. After, the projections of the features by teammates and rival team players were summed up, which brought symmetry for everyone.

For Data Augmentation; spatial features like coordinates were flipped with respect to X axis.
