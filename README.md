<h2 align="center"> Face-Recognition-Using-Face Net </h2>

## Introduction

* After all the advancements in the field of Computer Vision, implementing face verification and recognition efficiently at scale presents serious challenges to current approaches. This project presents a unified system for face verification, recognition, and clustering. 
* Deep convolutional networks are used to produce Euclidean 128-D embedding per image using a triplet-based loss function.
* Based on the learnings from these embeddings the fore mentioned tasks can be performed using techniques like thresholding (verification), KNN classification (recognition), and agglomerative clustering (clustering).

## Challenges
* The project is purely data-driven which learns its representation directly from the pixels of the face unlike other projects 1,2 that employ deep networks. 
* A large dataset of labeled faces is used to attain the appropriate invariances to pose, illumination, and other variational conditions rather than depending on the engineered features.

## Proposed Methodology
A network that consists of a batch input layer and a deep CNN followed by L2 normalization, which results in the face embedding followed by the triplet loss during the training. The triplet loss minimizes the distance between an anchor and a positive, both of which have the same identity, and then maximizes the distance between the anchor and the negative of the different identities.

<img src = "https://github.com/msc-1729/Face-Recognition-Using-FaceNet/blob/main/assets/Proposed%20Methodology.png" />


