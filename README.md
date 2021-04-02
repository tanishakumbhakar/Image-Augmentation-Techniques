# Image-Augmentation-Techniques
Dataset used consists of total 500 images of landslide downloaded from google.<br>
The training dataset consists of 400 images (80 % of total dataset), validation dataset consists of 50 images (10 % of total dataset), test dataset consists of 50 images (10 % of total dataset).<br>
For classification, a convolutional neural network with 32, 64 and 128 layers is used.<br>
The model is trained for 20 epochs, the accuracy values and loss values are noted and the best augmentation technique for our dataset is determined.<br>
The accuracy and loss values of different augmentation techniques after 20 epochs are:<br>
## 1. Random rotation
rotation_range=40,fill_mode='nearest'<br>
Accuracy: 0.92 <br>
Loss: 0.25<br>
## 2. Random shifts
width_shift_range=0.2, height_shift_range=0.2<br>
Accuracy: 0.74 <br>
Loss: 0.48 <br>
## 3. Random flips
horizontal_flip=True, vertical_flip=True<br>
Accuracy: 0.86 <br>
Loss: 0.41 <br>
## 4. Random zoom
zoom_range=0.2<br>
Accuracy: 0.60 <br>
Loss: 0.62 <br>
      
Thus, we can see on our dataset the best augmentation technique is Random rotation.
