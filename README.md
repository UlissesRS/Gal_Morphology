# Gal_Morphology
A repository where I comment my studies and progress during my master's degree towards data science and Galaxy Morphology applied to the DR3 of the Southern Photometric Local Universe Survey (S-PLUS).

In the first semester of 2021 the research group I was going to enter released an [article](https://arxiv.org/abs/2104.00018) where they classified galaxies of the Data Release 1 (DR1) of S-PLUS using deep learning. They had a plan to use the DR3 to extend the catalogue generated and to present some new features concerning the neural network. Then in the second semester I was invited to work in this project, something that would introduce me to the area of Big data, Data Science, Deep learning and Astronomy.

Naturally when dealing with deep learning we needed a big set of labeled images to serve as training for the model. Most of the time this data has to pass first for some processing such as pixel enhancement, normalization, before serving properly as training. Once it's done the model can be trained and some metrics can be used to evaluate its performance during the training and in the after training. The project was concepted using the library TensorFLow in Python that counts with a variaty of methods to calculate those metrics. In order to ilustrate it I leave below some figure showing the Loss function of the model, that essentially determines a distance between the predicted classifications and the actual classifications.

{image}

It's important to notice that 7 lines were drawn and that happened because the training was made using the cross validation k fold method. In this procedure the training is separated in k folds and for each fold we split the training in actual-training and validation, leaving no intersection between the validation of each fold. Then 7 models were trained with their particular performances that can be evaluated. Another thing interesting is to take the mean value between these folds
as the mean performance of the model and to take the standard deviation as uncertainty. 

This result can be achieved with this code: 
```
code here

```
{image}



