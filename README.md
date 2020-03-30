# Text-Summarization-using-Sequence-to-Sequence-LSTM
Our model represents abstractive text summarization using LSTM (Long-Short term memory network) based deep learning as a sequence-to-sequence model noting that this is many-to-many problem. Textual data is learned by using word embedding on the news article dataset to pertain the original meaning of the article. This contains the sequence to sequence model for text summarization which has given around 84% accurate summary for given text.

Table of Contents
•	General Information
•	Technologies
•	Setup

General Information
We have presented the model for summarization of text on news summary dataset. The model has performed with the accuracy around 84.63%. In this model, dropout and recurrent dropout used with LSTM layers played major role in resolving overfitting issue which provided comparatively better result. Experimental analysis shows that increasing the maximum text length as well as maximum summary length resulted to give more accuracy by 10%. This analysis aims on comparing the performance in training a deep learning model with new versus using pretrained word embeddings, where GloVe word embeddings has performed 40% better than new word embeddings which can be considered as a significant improvement in the sequence to sequence model on news summary dataset.

Technologies
Project is created with:
•	Windows 10 operating system
•	Colab Jupyter notebook
•	Dataset

Setup
The News Summary dataset which is collection of articles from Hindu, Indian times and Guardian that has been used to work on the project can be found at this below link: https://www.kaggle.com/sunnysai12345/news-summary

Steps to run the code:

1. Open ‘3_Project_2_TT.ipynb' file in python notebook platform like jupyter notebook or Google colab platform.
2. You will need GloVe word embeddings file which can be downloaded from https://www.kaggle.com/terenceliu4444/glove6b100dtxt .
3. A trained model with the weights can be found in ‘3_Project_2_TT.json' and '3_Project_2_TT.h5' files. JSON file is been uploaded , however for h5 file comment line 422 and run the whole model post which "3_Project_2_TT.h5" will be saved in the given path. 
4. You can load the trained model with the help of json file, but you will also need to load the weights for the trained model through h5 format file. You can find the code for loading the trained model and running it in last cell of the notebook. It will give you the validation accuracy on testing dataset.
5. To get the processed testing dataset, you need to run till the cell where we have performed padding of the sequences just before importing GloVe word embeddings.
