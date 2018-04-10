# KaggleDSBowl2018
MaskRCNN for Nuclei Detection on Google Colab

This kernel implements the following:

1. MaskRCNN implementation at https://github.com/killthekitten/kaggle-ds-bowl-2018-baseline#kaggle-ds-bowl-2018 in Jupyter Notebook form.
    - No change in code, only changed modules train.py and inference.py into procedures so they can be run within this notebook and take parameters
    - Using this code made 6 submissions after every 5 epochs going upto 35 epochs (5, 10, 15, 20, 25, 30, 35). Scores increased on LB until 20 epochs, then went down (probably overfitting). Max LB score at 20 epochs = 0.382
    
2. Be able to run this notebook in Google Collaboratory (https://colab.research.google.com/) and utilize the free GPU support. (Takes an average 10 minutes to run 1 epoch with GPU)
    - Loads all the competition data from Kaggle into Google Colab (the virtual environment allocated to the user)
    - Loads the model weights as required by the item 1 above into Google Colab
    - Loads the code from github for item 1 implementation
    - Can make competition submissions to Kaggle site directly from Google colab
    - After every 5 epochs during RCNN training uploads h5 weights file to your Google drive
