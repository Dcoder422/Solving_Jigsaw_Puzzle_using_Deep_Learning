# Solving_Jigsaw_Puzzle_using_Deep_Learning
This project is a part of Machine Learning competition, "MLWare'23" , organized under Technex'23 , the technomanagent fest of IIT BHU. We secured overall 3rd poition.

### The Problem Statement was based on Permutation Learning.

Given a jumbled sequence of elements, permutation learning aims to train a parametric model that can output the correct sequence of elements. Permutation learning is used to train models to learn rich features/representations of the elements of a sequence which can then be used to fine tune models on various downstream tasks. We use permutation learning in the context of Computer Vision where feature learning is of utmost importance

25th Feb 2023 to 19th Mar 2023

## 🔗 Links
[kaggle competion link here](https://www.kaggle.com/competitions/mlware23/overview)

[Presentation link Here](https://drive.google.com/file/d/1z20EF2lWrfOpG8ubfnmLOCAGMa2fD200/view?usp=sharing)

### Teamname : Prompt Engineers

Team Members
- Dhruvi Jain
- Sarthak Jain

## Tools and Techniques Used
- Implemented CNN using Tensorflow, to arrange shuffled pieces of face and landmark images into correct sequence.
- Performed Zero Padding to preserve all the edge features of the puzzle pieces. The model gave 88% accuracy for faces and 82% accuracy for landmarks.
- After trying many architectures we finally used 3 Convolutional hidden dense layers, with relu as activation function. 
- We performed Batch Normalization after passing image through each convolution layer.
- Performed Max Pooling of Pool Size (2,2) after each Batch Normalisation Step.

## Problems we faced
### *RESOURCE EXHAUSTED ERROR* 
- Due to the large size of data, while training deep model we were getting resource exhausted error. This was the reason why we couldn't add 4th convolution layer. Also, we couldn't increase the number of filters to extract more information especially in the case of Landmarks as its features are more complex than Faces. Even on decreasing kernel size, we had to deal with the same issue.

### Ranked 3rd among 90 teams in Final Round

## APPLICATION OF OUR SOLUTION
- Can be used in robots' intelligence system for contructive and management use cases.
- Our Solution can be used by archaeologiststo figure out the structure of artefactsfrom its broken and jumbled pieces.
- Our method can provide significant aid to archaeologists by cutting down the number of plausible reassemblies.
- Can be used in Investigations involving jumbled clues.
