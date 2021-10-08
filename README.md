# Pneumonia-Image-Classifier
This is a binary image classifier trained using a Convolutional Neural Network to differentiate between chest xrays of patients with or without Pneumonia. It was trained on a dataset of 5216 images taken from this kaggle dataset: https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia . This project is an example of how useful machine learning and computer vision techniques can be for the medical field.


## Methods
This model uses a combination of Conv2D, MaxPooling2D, and a Dense layer with dropout feeding into a sigmoid layer. The loss function used is binary crossentropy. Basic image manipulations are performed on the data before being fed into the model to add diversity to the images trained on. Using these methods, the model achieved a validation accuracy of 87% with a test accuracy of 97.3%. This was confirmed by increasing the default validation set from 16 images to 80 using data removed from the training set. A further 20% of the training set was then set aside for testing, as there seems to be inaccurate labeling in the original test set.

## Future Work
This project has achieved a high accuracy but extensive hyperparameter optimization hasn't been done to find the ideal capacity or other parameters for the network. Next steps may involve modifying the classifier to run on accelerated hardware such as GPUs and TPUs to save training time and better enable deployment in cloud environments.
