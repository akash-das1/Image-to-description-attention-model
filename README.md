EYE FOR BLIND
This notebook will be used to prepare the capstone project 'Eye for Blind'
Our primary objective is to generate caption for a provided image. We will use CNN-RNN based Attention model to achive this goal.
We have used flicker8k images along with around 5 different types of captions.
CNN will create a feature map evaluating traing images aganist provided caption and with help of RNN (gru here) we generate the captions.
We We have used gredy search approch to generate the caption and evaluated the result using BELU score.
There are more indepth work involved here as part of saving featuremap to reuse, Attention model with Teacher forcing to achive better results, etc.
- Here we have 2 parts,
          1. create the feature map and 
          2. Use it in Attention model.
So, if we are running this file first time, we need to keep 'Create_image_features = True' to save the mapping file on storage. Later we will mark it False, not to generate the map again and reuse the mapping file generated in first run.

Also, we are running it on Goggle colab and we should make sure to have 10GB of available space torun it sucessfully. In 3rd cell, please update the path of the storage which will contain 'Image' folder for traning images and other files outside of image folder. IITB_Capstone > Data > Images
