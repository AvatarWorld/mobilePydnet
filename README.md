# PyDNet on mobile devices

[![Build Status](https://travis-ci.org/FilippoAleotti/mobilePydnet.svg?branch=master)](https://travis-ci.org/FilippoAleotti/mobilePydnet)

This repository contains the source code to run PyDNet on mobile devices (`Android` and `iOS`)

If you use this code in your projects, please cite our paper:

```
@inproceedings{pydnet18,
  title     = {Towards real-time unsupervised monocular depth estimation on CPU},
  author    = {Poggi, Matteo and
               Aleotti, Filippo and
               Tosi, Fabio and
               Mattoccia, Stefano},
  booktitle = {IEEE/JRS Conference on Intelligent Robots and Systems (IROS)},
  year = {2018}
}
```

More info about the work can be found at these links:
* [PyDNet paper](https://arxiv.org/pdf/1806.11430.pdf)
* [PyDNet code](https://github.com/mattpoggi/pydnet)

## Model
The network has been trained on [MatterPort](https://matterport.com/it/) dataset for 1.2M steps, using the BerHu loss on Microsoft Kinect depth labels offered by the dataset as supervision.

<p align="center">
  <img src="images/im0.jpg" width="300" height="500"/>
  <img src="images/im1.jpg" width="300" height="500"/>
</p>

## Android
The code is based on [Google android examples](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/examples/android).
Android `target` version is 26 while `minimum` is 21. Android Studio is required.

Currently, we use `tensorflow-android` instead of `tf-lite`, and no gpu-optimisation is supported.

**Mode**: portrait

### Android Examples

<p align="center">
  <img src="images/im2.jpg" width="300" height="500"/>
  <img src="images/im3.jpg" width="300" height="500"/>
</p>

## iOS
The demo on iOS has been developed by [Giulio Zaccaroni](https://github.com/GZaccaroni).

XCode is required to build the app, moreover you need to sign in with your AppleID and trust yourself as certified developer.

**Mode**: landscape

### iOS Examples

<p align="center">
  <img src="images/im4.png" width="300" height="500"/>
  <img src="images/im5.jpeg" width="300" height="500"/>
</p>

## Licenses

The code provided in this repository has a demonstrative and academic purposes only. Even if we released this code using Apache License v2, pre-trained model on specific datasets may not be used for scopes not covered by their licenses.

* [MatterPort’s](https://matterport.com/it/) license