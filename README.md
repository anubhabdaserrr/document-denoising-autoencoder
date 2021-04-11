# Removing background noise of text documents using denoising autoencoder

**Project Report by Anubhab Das** 

Date : 10th April, 2021

[![nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.jupyter.org/github/anubhabdaserrr/document-denoising-autoencoder/blob/main/doument_denoising_autoenc_nb.ipynb)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/anubhabdaserrr/document-denoising-autoencoder/blob/main/doument_denoising_autoenc_nb.ipynb)

## Objective & data

![](./misc/train_imgs_1.png)
![](./misc/train_imgs_2.png)

**Note : In the context of this project, denoising refers to removal the content of the background (which may not necessarily be "noise" but is treated in this work as such) to successfully extract the foreground text.**

## Model & Training details

### Convolutional Autoencoder Architecture
![](./misc/autoenc_arch.png)

### Training details
```
Optimizer : Adam with mini-batch gradient descent
beta1 : 0.999
beta2 : 0.999
Learning rate : 0.01 
Loss : Mean Squared Error
Validation Metric : Mean Absolute Error
Mini batch size : 32
No. of epochs : 100
```

## Evaluation & test performance

### Loss Curves :
<img src="./misc/mse_loss_curve.png" width="418" height="282" /> <img src="./misc/mae_curve.png" width="418" height="282" />

### Validation Predicted & Actual Images :
![](./misc/val_imgs_pred_3.png)
![](./misc/val_imgs_pred_4.png)


### Validation Images Pixel Intensity Histograms :
![](./misc/pixel_hist_valpred3.png)
![](./misc/pixel_hist_valpred3.png)

### Denoising unseen test images :
![](./misc/test_pred_1.png)
![](./misc/test_pred_2.png) 
![](./misc/test_pred_3.png) 

## References
Links go here
