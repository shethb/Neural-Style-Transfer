# Neural-Style-Transfer

An implementation of neural style in TensorFlow.

I have used pre-trained VGG-19 network and then gave three input images, Style Image, Content Image and an image that is initialized to white noise. VGG-19 model has already been trained on the very large ImageNet database and thus has learned to recognize a variety of low-level features (at the earlier layers) and high-level features (at the deeper layers). Thereafter I have created cost function that minimizes content loss and style loss. Optimizing the total cost function results in synthesizing the new images.

Running it for 500-2000 iterations seems to produce nice results. With certain images or output sizes, you might need some hyperparameter tuning (especially --content-weight, --style-weight, and --learning-rate).

The following example was run for 1000 iterations to produce the result (with default parameters):

Original Image of ice hockey:

![Original Image](original_image.jpg)

The art image I have used to transform the original image is:

![Art Image](art_wallpaper.jpg)

The transformed image is:

![Deep Art Image](deepart_image.png)

