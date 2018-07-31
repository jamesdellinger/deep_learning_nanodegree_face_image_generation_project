# Project: Generate New Images of Faces using Deep Convolutional GANs
*Training a generative adversarial network to generate new, unique images of human faces that are often indistinguishable from images of real individuals' faces.*

<img src="https://github.com/jamesdellinger/deep_learning_nanodegree_face_image_generation_project/blob/master/dlndlogo.png" height="140">

For Udacity's [Deep Learning](https://www.udacity.com/course/deep-learning-nanodegree--nd101) Nanodegree.

Topic: Generative Adversarial Networks.

## Overview
* I used TensorFlow to build and train a deep convolutional GAN that is able to generate life-like images of human faces after one training epoch.
* I first tweaked my generator and discriminator network architectures, and values of hyperparameters such as batch size, while training the networks on the [MNIST](http://yann.lecun.com/exdb/mnist) handwritten digits dataset, getting them to they place where could generate decent looking handwriting samples.
* I then trained my GAN using the 200,000 celebrity face images in the [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) dataset.
* After further decreasing the learning rate, my GAN was able to generate reasonably convincing images resembling human faces after only one training epoch:
  <img src="https://github.com/jamesdellinger/deep_learning_nanodegree_face_image_generation_project/blob/master/generated_faces.png" height="140">
* The [MNIST](http://yann.lecun.com/exdb/mnist) dataset is maintained courtesy of [Yann LeCun](http://yann.lecun.com), [Corinna Cortes](http://homepage.mac.com/corinnacortes), and [Christopher J.C. Burges](http://research.microsoft.com/en-us/people/cburges).
* The [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) dataset comes from [Ziwei Liu](http://personal.ie.cuhk.edu.hk/~lz013), [Ping Luo](http://personal.ie.cuhk.edu.hk/~pluo), [Xiaogang Wang](http://www.ee.cuhk.edu.hk/~xgwang), and [Xiaoou Tang](http://www.ie.cuhk.edu.hk/people/xotang.shtml) of the [Multimedia Laboratory](http://mmlab.ie.cuhk.edu.hk) of The Chinese University of Hong Kong.

## Concepts
* Deep Convolutional GAN architecture.
* Successive [conv2d_transpose](https://www.tensorflow.org/api_docs/python/tf/layers/conv2d_transpose) layers in the generator network, in order to create unique, convincing 2d images based on a random input signal.
* Using batch normalization to stabilize GAN training by reducing internal covariant shift.

## My Completed Project
* [ipython notebook](https://github.com/jamesdellinger/deep_learning_nanodegree_face_image_generation_project/blob/master/dlnd_face_generation.ipynb) / [html version](https://github.com/jamesdellinger/deep_learning_nanodegree_face_image_generation_project/blob/master/dlnd_face_generation.html) / [pdf version](https://github.com/jamesdellinger/deep_learning_nanodegree_face_image_generation_project/blob/master/dlnd_face_generation.pdf)

## Project Grading and Evaluation
* [Project Review](https://github.com/jamesdellinger/deep_learning_nanodegree_face_image_generation_project/blob/master/face_image_generation_project_review.pdf)

* [Project Grading Rubric](https://github.com/jamesdellinger/deep_learning_nanodegree_face_image_generation_project/blob/master/face_image_generation_project_grading_rubric.pdf)

## Dependencies
* [requirements.txt](https://github.com/jamesdellinger/deep_learning_nanodegree_face_image_generation_project/blob/master/requirements.txt)
