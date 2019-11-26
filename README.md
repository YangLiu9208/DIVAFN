## Deep Image-to-Video Adaptation and Fusion Networks for Action Recognition  
(accepted by IEEE Transactions on Image Processing)  

<a href="https://orcid.org/0000-0002-9423-9252" target="orcid.widget" rel="noopener noreferrer" style="vertical-align:top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" style="width:1em;margin-right:.5em;" alt="ORCID iD icon">orcid.org/0000-0002-9423-9252</a>

Homepage: [https://yangliu9208.github.io/home/](https://yangliu9208.github.io/home/)

## Abstract
Existing deep learning methods for action recognition in videos require a large number of labeled videos for training, which is labor-intensive and time-consuming. For the same action, the knowledge learned from different media types, e.g., videos and images, may be related and complementary. However, due to the domain shifts and heterogeneous feature representations between videos and images, the performance of classifiers trained on images may be dramatically degraded when directly deployed to videos without effective domain adaptation and feature fusion methods. In this paper, we propose a novel method, named Deep Image-to-Video Adaptation and Fusion Networks (DIVAFN), to enhance action recognition in videos by transferring knowledge from images using video keyframes as a bridge. The DIVAFN is a unified deep learning model, which integrates domain-invariant representations learning and cross-modal feature fusion into a unified optimization framework. Specifically, we design an efficient cross-modal similarities metric to reduce the modality shift among images, keyframes and videos. Then, we adopt an autoencoder architecture, whose hidden layer is constrained to be the semantic representations of the action class names. In this way, when the autoencoder is adopted to project the learned features from different domains to the same space, more compact, informative and discriminative representations can be obtained. Finally, the concatenation of the learned semantic feature representations from these three autoencoders are used to train the classifier for action recognition in videos. Comprehensive experiments on four real-world datasets show that our method outperforms some state-of-the-art domain adaptation and action recognition methods.

## Network architecture
![Image](Network_image.png)

Figure 1: Configuration of the deep neural network for image modality. "f" denotes the number of convolutional filters and
their receptive field size, "st" denotes the convolutional stride, "pad" denotes the number of pixels to add to each size of the
input, "LRN" denotes whether Local Response Normalization (LRN) is applied or not, and “pool” denotes the downsampling factor.

![Image](Network_image.png)

Figure 2: Configuration of the deep neural network for keyframe modality. 


![Image](Network_video.png)

Figure 3: Configuration of the deep neural network for video modality

## Datasets

![Image](Datasets.png)

Stanford40->UCF101 dataset can be downloaded here. [Stanford40](https://drive.google.com/open?id=1f8XJ-GSIrB1fJFZJzgECYA6w9-OJWiJr)

ASD->UCF101 dataset can be downloaded here. [ASD](https://drive.google.com/open?id=1xor9cfZ-ny-OfBbTnKRR_6oQyebKkD-g)

EAD->HMDB51 dataset can be downloaded here. [EAD](https://drive.google.com/open?id=11GghjBp1jgFKDwvudZGLzPbSuCP4DJfs), [HMDB51](http://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/)

BU101->UCF101 dataset can be downloaded here.   [BU101](http://cs-people.bu.edu/sbargal/BU-action/), [UCF101](http://crcv.ucf.edu/data/UCF101.php)


## Codes
Soon will be available.

<a href='https://clustrmaps.com/site/1b049'  title='Visit tracker'><img src='//clustrmaps.com/map_v2.png?cl=ffffff&w=a&t=m&d=GnHm4-dMEE6iXqoDt0fhb1JfsnTDg8p0HALKu6yPxDc&co=2d78ad&ct=ffffff'/></a>
