---
layout: page
title: Machine Learning @ Alice
permalink: /ml/
---

# Welcome to Alice - the Datahub of MediaMarktSaturn!


As we try to use newest technology with Alice - we're focusing on machine learning as one key goal in bringing new techonolgy to live within our company. 

This page should give an idea of what we're expering on this journey and how we try to solve problems with the help of ML. 


---

## Abstract of Google Machine Learning Advanced Solution Lab - Dublin (09.04.2018 - 04.05.2018)

> With this abstract we want to share our experience and knowledge, we build up during the ASL in Dublin, 
> where we spend 1 month practicing and expanding our knowledge about machine learning.


At first, we got an Introduction to Datalab, a cloud-native programming environment for data scientists, 
and were shown how cloud technologies can be used to easily, quickly, and collaboratively analyze massive datasets.
After that we focused on the theory of ML - What is ML? What questions do we need to ask if we want to bring ML into our business? 
- We had to answer a question framework for a specific problem we want to solve with ML within our company which looks like that:

![alt text](pics/table.png "ML - Decission Table")


Whereas this table tries to help companies to figure out whether their problem is a real ML problem and how to split this, 
it is very important that everyone within the company as the understanding of ML as the last step of data analysis and is more a journey than a simple task. The steps of this journey are shown in the following picture as a pyramide:


![alt text](https://github.com/EastOfGondor/documentation/blob/master/pics/pyramide.png)

![alt text](https://github.com/EastOfGondor/documentation/blob/master/pics/pyramide5.png "ML - Pyramide")


When the understanding is clear you can start to ask yourself what kind of ML problem you have. 
Therefore we were introduced the two main categories of ML:

* Supervised Learning
* Unsupervised Learning

This course was designed to make a deep dive into supervised learning and the both subcategories “Regression” and “Classification”.

There are different types of algorithms for different types of approaches - so you have to know what you want to achieve when tackling an ML problem. We were introduced to different algorithms of the both subcategories which can solve most of the “known” ML Tasks which are e.g. recommendation engine, forecasting, image classification, natural language processing, logistic and linear regression.

To solve all these problems we used one of the most famous and fastest ML libraries nowadays “TensorFlow”. It offers a bunch of methods to interact with all of these algorithms and it was one of the main goals during the course to get familiar with all of the frameworks advantages.

We covered the whole ML journey a lot of times during different labs where we had a closer look in almost each of the named algorithms and lastly also build up our own project.
Almost every ML journey looks like this:

![alt text](https://github.com/EastOfGondor/documentation/blob/master/pics/end_to_end.png "ML - end to end journey")

Every ML Problem begins with Data - which is the key success factor for each ML solution. Without “good and suitable” ML is impossible. So we had every time our first look at the data. Therefore we used the following solutions of GCP:

* Cloud Datalab 
* BigQuery
* Dataprep

For the development of a “good” model, the whole dataset has to be splitted into a train, evaluation and eventually a test dataset. Once you are done with the training, you need to check how well your model is doing, therefore evaluation and test dataset is used .

For the first models you develop you don’t use the whole dataset which should usually contain millions of rows - to safe money and time. To create this datasets we used the following GCP tools:

* Cloud Dataflow
* BigQuery
* Cloud Storage
* Cloud Datalab

After that it’s time to develop the first model with Tensorflow in Python. The framework offers the usage of predefined model estimators which means the model structure is build by default and can be used to fill it which specific parameters which fit to your problem and your data. Here are a few examples of the algorithms and how we implemented them in Tensorflow:

![alt text](https://github.com/EastOfGondor/documentation/blob/master/pics/wide_deep_models.png "Wide and Deep models")

![alt text](https://github.com/EastOfGondor/documentation/blob/master/pics/wide_deep_code.png "Tensorflow Code - Wide and Deep model")

After the model was developed it can be trained with the sample dataset, local. With the training comes the art and science: Involving knowledge of the right mix of parameters that
yields accurate, generalized models and a science involving knowledge of the theory to solve specific types of ML problems.
		
If the model - with the sampled data - fits our expectations, we can shift training into the cloud and use the whole dataset to improve our model. To use this big bunch of data in the cloud we need to build a special input pipeline - otherwise training would takes months to finish. This pipeline enables the ML Engine to paralyse the training and speed it up extremely.

Another key aspect the cloud ML Engine can help us with, is hyperparameter tuning, which means that you specify a range for each of your model parameters and MLEngine in GCP figures out for which combination of different parameter values the model performs best. This means that it it will show you the parameters for which the model has its lowest loss.

Once the best parameters for the model are found, the model can be deployed within ML Engine to make predictions. Therefore it offers an API which can be used to make stream and batch predictions from everywhere - also mobile.

This was a short abstract of what we’ve learned and experienced during Google ASL. The training was totally worth it and we have deepen our knowledge around ML topics and Google Cloud Platform extremely. We also made the experience that GCP is an enabler of ML in every single step - the whole platform is designed to make the life of an ML-Engineer easier and faster.

We’re open to share all of our knowledge with everyone within the company and push ML in our own projects. Thank you all of our sponsor that gave us the possibility to get this experience.

Daniel Budick, Josef Goppold, Tobias Hoke, Fabian Seitz




---

