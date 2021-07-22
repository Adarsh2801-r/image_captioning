# Image Captioning
Dataset-https://drive.google.com/drive/u/0/folders/1ysngnEgkyVu1AHaDk34-15YuavSVXIBB <br>
**Introduction** <br>
Image description generation or image captioning is the process of generating sentences related to a given image. Image description generation has a wide range of uses, like image indexing, accessibility for visually impaired people, social networking, search engines and recommendation systems. Image description generation can be considered an end to end seq2seq problem because it deals with the conversion of images (sequence of pixels) to sentences (sequence of words). We have used an encoder-decoder network to generate the captions for the images. In the encoder part, we have used convolutional neural networks (CNNs) to extract the features from the images and in the decoder part, we have used transformers to generate the captions.<br>

**About the project** <br>
We created a sentence-based image description generator; this project comes under two flourishing domains of deep learning image recognition and natural language processing. First, we generated index-based encoding of the captions present in the dataset our model uses these text encodings to train on. We then used the pre-trained ResNet models to extract image embeddings which we used as input to transformers’ decoder layer, which uses these image embeddings to generate sentences that describe the image. <br>


**Workflow followed:**
1. Collected data
2. Performed Data Augmentation
3. Word/Sentence Embedding
4. Combined Model
> 4.1 CNN for encoding-ResNet <br>
> 4.2 Transformers for decoder network <br>
> 4.3 Combined Loss and Fine Tuning <br>
5. Validation of Description
6. Generalization/Decoupling of Code
