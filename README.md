# How to train YOLOv3 using Darknet on Colab 12GB-RAM GPU notebook and optimize the VM runtime load times

This repo contains the Google Colab Notebook based off of[this post]((http://blog.ibanyez.info/blogs/coding/20190410-run-a-google-colab-notebook-to-train-yolov3-using-darknet-in/) by :

This Colab notebook will show you how to:

* Train a **YOLOv3** model using **Darknet** using the Colab **12GB-RAM GPU**
* Sync Colab with your Google Drive
* See how to configure **YOLOv3** training on an example dataset

# Notebook 1: DarknetYOLOTrain_Init.ipynb

This notebook covers the setup of darknet and initial training (approx. 12 hours) with the provided dataset and config files.

1. Connecting between Google Drive and Colab for file storage
2. Install of CUDA cuDNN library
3. install of darknet on Colab and storage of compiled darknet binary on Google Drive for later reuse
4. importing config and training data images from Google Drive
5. Downloading initial pretrained weights
6. Training model and storing trained weights in Google Drive

# Notebook 2: DarknetYOLOTest.ipynb

1. Reloading model from weights from Google Drive
2. Using model weights to perform object detection on an example file


# Notebook 3: DarknetYOLOTrain_Repeat.ipynb

This notebook is similar to Notebook 1, but reuses the previously saved binaries and data to quickly reinitialize the runtime for repeated training.


## Credits

For this example, I simplified the tutorial from [this repo](https://github.com/kriyeng/yolo-on-colab-notebook) by [David Ibáñez](https://github.com/kriyeng). You can find the original post with more explanations about this notebook at [How to train YOLOv3 using Darknet framework and optimize the VM runtime load times](http://blog.ibanyez.info/blogs/coding/20190410-run-a-google-colab-notebook-to-train-yolov3-using-darknet-in/)

* You can visit ibanyex's blog at [Dev-ibanyez.info](http://blog.ibanyex.info)
* You can get in touch with me on [Twitter](https://twitter.com/dav_ibanez)
