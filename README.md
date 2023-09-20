# Image similarity learning using PyTorch -

This repository explores two of the popular methods for image similarity, siamese network and triplet network.
It is quiet challenging to implement these methods, given the typr of data required by models and the loss function, plus, the way of customizing models. 
Siamese networks aim to learn embeddings by making use of a similarity metric. Contrastive loss (there are alternatives) is used as a loss function in siamese network, which minimizes the distance between embeddings of similar pairs and maximize the distance between embeddings of dissimilar pairs. Siamese networks are trained using pairs of images, where each pair consists of two images and a flag indicating whether they are similar or dissimilar.

Notebook using siamese - 
'''
contrastive.ipynb
'''

Triplet networks also aim to learn embeddings, but they use a triplet loss function. The idea is to learn embeddings in such a way that the distance between an anchor image and a positive (similar) image is smaller than the distance between the anchor image and a negative (dissimilar) image. Triplet networks are trained using triplets of images, an anchor, a positive example (similar to the anchor), and a negative example (dissimilar to the anchor).

Notebook using triplet - 
'''
triplet.ipynb
'''

### To learn more about this methods -
#### Siamese networks-
- [https://en.wikipedia.org/wiki/Siamese_neural_network](https://en.wikipedia.org/wiki/Siamese_neural_network)
- [https://jamesmccaffrey.wordpress.com/2022/03/17/yet-another-siamese-neural-network-example-using-pytorch/](https://jamesmccaffrey.wordpress.com/2022/03/17/yet-another-siamese-neural-network-example-using-pytorch/)
- [https://github.com/pytorch/examples/tree/main/siamese_network](https://github.com/pytorch/examples/tree/main/siamese_network)
- [https://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf](https://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf)
- [https://gowrishankar.info/blog/introduction-to-contrastive-loss-similarity-metric-as-an-objective-function/](https://gowrishankar.info/blog/introduction-to-contrastive-loss-similarity-metric-as-an-objective-function/)
- 
#### Tripet network-
- [https://en.wikipedia.org/wiki/Triplet_loss](https://en.wikipedia.org/wiki/Triplet_loss)
- [https://arxiv.org/abs/1412.6622](https://arxiv.org/abs/1412.6622)
- [https://github.com/adambielski/siamese-triplet](https://github.com/adambielski/siamese-triplet)


There are other methods too, for the task of finding similar images. Check out this competition hosted on [drivendata](https://www.drivendata.org/competitions/group/meta-vsc-open-arena/) by Meta AI. The winning solutions used self-supervised learning to detect whether a query video contains manipulated portions of one or more videos in a reference set. The dataset provided is very interesting, heavily edited, which would require novel solutions and heavy augmentations to perform well on the metric used to measure models performance.


## Dataset-
Dataset used can be found [here](https://www.kaggle.com/datasets/stoicstatic/face-recognition-dataset)



# To do -

- [ ] Convert to python script
- [ ] Explore other methods
- [ ] Demo using streamlit