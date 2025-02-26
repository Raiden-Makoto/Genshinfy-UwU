# Siamese Network for Image Similarity Estimation
The goal: given a database of anime images and an image of the user's face, return the top 5 anime characters that most closely resemble the user's face. This model is trained on the custom human-anime dataset located in the `SiameseData` folder.  

### Description
The Siamese Network is a modifed version of `ResNet50` pretrained on ImageNet; the model is connected to a few Dense layers so we can learn to separate the embeddings of each of the images in the triplet `(anchor, positive, negative)`. The model is trained with **Triplet Loss** and uses **Cosine Similarity** to determine the best match for the input image.
