# Pokemon Classification - Gen I

Dataset: [7000 hand-cropped and labeled Pokemon images for classification](https://www.kaggle.com/lantian773030/pokemonclassification)

Project 2 for Machine learning course for Software and Knowledge Engineering, Kasetsart University

### Prerequisite
- Python >= 3.6
- Cuda

install required libraries
```sh
pip install -r requirements.txt
```
run jupyter notebook
```sh
jupyter notebook
```

-----

## Progressive resizing
reference: [Boost your CNN image classifier performance with progressive resizing in Keras](https://towardsdatascience.com/boost-your-cnn-image-classifier-performance-with-progressive-resizing-in-keras-a7d96da06e20)

## Report Finding
7000 samples across 150 classes is not enough for training a good model expecting a generalized high accuracy model.
I decided to implements a progressive resizing technique to helps improve the gerneralability and got a pretty good result.
The trained model have the accruracy around 70-80% with minor confusion when encounter a very similar pokemon 
like _Mankey_ and _Primeape_

The area that I think my project could be improve is train, eval, and test data split could be done better.
If the dataset is better splitted I can smooth out the evaluation accuracy and evaluation loss.
