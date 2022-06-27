# cuisine-recommendation-ml-model

What if you wanted to determine whether a given cuisine was likely to use fenugreek? What if you wanted to see if, given a present of a grocery bag full of star anise, artichokes, cauliflower, and horseradish, you could create a typical Indian dish? 

This cuisine recommendation machine learning model predicts a given national cuisine based on a group of ingredients using the Linear SVC Classification Model. The dataset used is cuisines.csv which contains 380 ingredients. 

In the clean_data.ipynb notebook, the data is cleaned and balanced. The distribution of data is examined and recurrent data is cleaned. Using Synthetic Minority Over-sampling Technique (SMOTE), the data is balanced to gain better results during classification. This cleaned data is saved in cleaned_cuisines.csv.

In the classification_models.ipynb notebook, the cleaned dataset is used with a variety of classifier algorithms to predict a given national cuisine based on a group of ingredients. The classifiers used are Logistic Regression, Linear SVC Classifier, K-Neighbors Classifier, and Support Vector Classifier. For all these classifiers, the data is split into testing and training groups and the models are trained. The reports are printed and their accuracies are compared to decide which technique should finally be used to build the cuisine recommendation model. 

In the cuisine_recommender_model.ipynb notebook, the cuisine recommendation model is built using SVC Classification model. The cleaned dataset is used to build it. The model is converted to Onnx to enable developers to use it in a variety of different frameworks and tools.


# run the model
The cuisine_recommender_model.ipynb notebook can be accessed using Google Colab or cloned. On completing running this notebook, the model is stored as a file cuisine_recommender_model.onnx. Download Netron (https://github.com/lutzroeder/Netron) and open the cuisine_recommender_model.onnx file to see the model visualized, with its 380 inputs and classifier listed.
