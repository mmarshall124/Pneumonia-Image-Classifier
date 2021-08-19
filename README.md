# Pneumonia-Image-Classifier
This is a binary image classifier trained using a Convolutional Neural Network to differentiate between chest xrays of patients with or without Pneumonia. It was trained on a dataset of 5216 images taken from this kaggle dataset: https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia . This project is an example of how useful machine learning and computer vision techniques can be for the medical field.


## Methods
This is a mostly unoptimized model using a combination of Conv2D, MaxPooling2D, and a Dense layer with dropout feeding into a sigmoid layer. The loss function used is binary crossentropy. Using these methods, the model achieved a validation accuracy of 97.5% with an expected test accuracy around 70-80%.

## Future Work
This project is still very early on in it's lifecycle. The model could be improved using image preprocessing techniques to add more diversity to the images trained on. The capacity and parameters of the model itself should also be heavily experimented with to find the optimal configuration and avoid overfitting. The classifier should also be modified to run on accelerated hardware such as GPUs and TPUs to save training time and better enable training in cloud environments.

Something that should be investigated is possible mislabled data in the final test set as theorized by some users on the dataset's discussion board. This may cause final accuracy ratings to be lower than expected based on training results.
