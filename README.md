## An Auto-Encoder based Object Recognition Framework for assisting the Visually Impaired.

<p align="justify">
An Object Recognition framework that uses low-level image features (Histogram of Oriented Gradients, Bag of Visual Words, and Local Binary Patterns) to learn high-level image representations using Auto-Encoders.
</p>

### Introduction

<p align="justify">
Vision is considered to be supreme among all other human senses. Impairment of vision impacts both physical as well as psychological aspects of life. Various devices have been proposed over time to assist the visually impaired in their daily lives. Among these devices, computer vision based solutions are most preferable due to accessibility and affordability. Most recently, Convolutional Neural Networks
(CNNs) have been used for object recognition in vision assistance devices. In contrast to earlier methods, which use manually extracted low-level image features, CNNs are able to automatically learn low-level and high-level features from images. It enables them to achieve higher recognition rates, but at the expense of larger computational costs. The goal of this project was to investigate an object
recognition method [1] that aims to reduce the amount of computation involved in the high-level feature learning process. The studied method uses Auto-Encoders (AEs) to transform low-level image features to high-level feature space representations. The performance of this method was compared with deep CNN based object recognition architecture.
</p>  

### Objectives
<p align="justify">
Mekhalfi et al. [1] proposed the use of AEs to transform low-level image features to high-level feature space representations. The primary objectives of this project were:

1. To reproduce the object recognition algorithm proposed in [1], and,
2. To compare the performance of the algorithm [1] with deep CNN based object recognition.
</p>

### Framework
<p align="justify">
The object recognition algorithm proposed in [1] first extracts Histograms of Oriented Gradients (HOG) [2], Bag of Words (BoW) [3] and Local Binary Patterns (LBP) [4] feature vectors from an image which are then mapped to their respective high-level feature spaces using AEs. The resulting high-level feature vector of each type is then fed into a separate Logistic Regression (LR) classifier. The output probability vectors from all three LR classifiers are averaged and thresholded to obtain list of predicted labels.
</p><br>

<p align="center">
<img src="https://github.com/msharm05/ae-ObjectRecognition/blob/master/Images/21.PNG" width=488 height=199>
</p>


  
