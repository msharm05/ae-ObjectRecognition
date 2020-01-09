## An Auto-Encoder based Object Recognition Framework for assisting the Visually Impaired.

<p align="justify">
An Object Recognition framework that uses low-level image features (Histogram of Oriented Gradients, Bag of Visual Words, and Local Binary Patterns) to learn high-level image representations using Auto-Encoders.
</p>

### Introduction

<p align="justify">
Vision is considered to be supreme among all other human senses. Impairment of vision impacts both physical as well as psychological aspects of life. Various devices have been proposed over time to assist the visually impaired in their daily lives. Among these devices, computer vision based solutions are most preferable due to accessibility and affordability. Most recently, Convolutional Neural Networks
(CNNs) have been used for object recognition in vision assistance devices. In contrast to earlier methods, which use manually extracted low-level image features, CNNs are able to automatically learn low-level and high-level features from images. It enables them to achieve higher recognition rates, but at the expense of larger computational costs. The goal of this project was to investigate an object
recognition method that aims to reduce the amount of computation involved in the high-level feature learning process. The studied method uses Auto-Encoders (AEs) to transform low-level image features to high-level feature space representations. The performance of this method was compared with deep CNN based object recognition architecture.
</p>  

### Objectives
<p align="justify">
Traditional object recognition methods and CNNs follow the same functional paradigm: image feature extraction followed by classification [14]. The two approaches differ primarily in their respective ways for extracting features. Traditional methods involve a hand-crafted feature extraction stage which produces low-level image features such as edges, corners, lines etc., whereas a CNN automatically learns complex features from images (e.g., shapes, textures) via successive convolutional layers [9]. In comparison to manually engineered features used in traditional methods, high-level features learned by a CNN yield better classification results. However, the learning process is highly expensive in terms of computation. Considering this limitation, Mekhalfi et al. [15] proposed the use of AEs to transform low-level image features to high-level feature space representations. The object recognition algorithm proposed in [15] first extracts Histograms of Oriented Gradients (HOG) [16], Bag of Words (BoW) [17] and Local Binary Patterns (LBP) [18] feature vectors from an image which are then mapped to their respective high-level feature spaces using AEs. The obtained high-level features are fed into a Logistic Regression classifier. The primary objectives of this project were:

1. To reproduce the object recognition algorithm proposed in [15], and,
2. To compare the performance of the algorithm [15] with deep CNN based object recognition.
</p>
