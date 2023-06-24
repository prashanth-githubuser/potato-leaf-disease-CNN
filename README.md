# potato-leaf-disease-CNN
Potato plant disease prediction using deep learning CNN architecture.

The data set consists of around 2144 files with 3 label namely Healthy, Early_blight and Late_blight.
Images are resized to 256,256 and normalized. Since the dataset is small, training data is augumented by flipping horizontaly and vertically  before fed in to the CNN architecture.

During training the validation loss, Training loss, Vlaidation accuracy and Training accuracy are logged in csv file for eeach epochs.
Started training with normal layers later the model is fine tuned by adding L2 regularization and changing the learning rate of optimizer.

Below are the obtained results.

__Trial-1__

<img src="/workspaces/potato-leaf-disease-CNN/trial Results/tial-1.png" alt="Image" width="400" height="200">

The model is started to overfit
--- 

__Trial-2__

<img src="/workspaces/potato-leaf-disease-CNN/trial Results/trial-2.png" alt="Image" width="400" height="200">

Model's validation loss is started to reduce after changing LR of adam optimizer 
---

__Trial-3__ : 

<img src="/workspaces/potato-leaf-disease-CNN/trial Results/trial-3.png" alt="Image" width="400" height="200">

After setting the optimizer learning rate and L2 values the Validation loss and model validaion accuracy is getting to optimum values 
--- 

Testing:

<img src="/workspaces/potato-leaf-disease-CNN/trial Results/Result -1.png" alt="Image" width="400" height="200">

Model performing well but predecting Healthy as Late_blight, This is due to very less Healthy label data points.

<img src="/workspaces/potato-leaf-disease-CNN/trial Results/Reslut-2.png" alt="Image" width="400" height="200">

<img src="/workspaces/potato-leaf-disease-CNN/trial Results/Result-3.png" alt="Image" width="400" height="200">

