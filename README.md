# Volumetric-Segmentation-of-3D-images

The repository consists of M.Sc.-Project-1(IE-689) that i did during my masters in IIT Bombay. The project has been under the guidance of Prof. N. Hemachandra and Prof. P Balamurugan. 

In computer vision, image segmentation is the process of partitioning a digital image into multiple segments. In 2D images, segmentation can be seen and visualized easily. But in case of 3D images, it is difficult to vizualise the images and the segmented images. Thus, in this project, firstly, various represantations of 2D and 3D images are revisited. Then, Segmentation has been done using [3D-Unet](https://arxiv.org/pdf/1606.06650.pdf).
**![](https://lh3.googleusercontent.com/W_R5qMQjniXdv4Orj1pmWYDTLQ2jhdBRWJwc2N2Egcn-sznTJNdpwK1tX2sjEG2qt2Gh0c5r8SKpQijHULRk4Ugisjr_2H_xWHMyyLvcxAy108mzXFht8Onm3pg_eVbwxFmLlGvW)**

## Data-set
The data-sets[1] that are used in this project are heart and spleen data-sets from Medicaldecation[1]. These data-sets have highly variable segmentation tasks that was used in a crowd-sourced challenge the Medical Segmentation Decathlon held during the 2018 Medical Image  Computing and Computer Aided Interventions Conference in Granada, Spain. It consists of a set of 10 different data-sets namely: Liver Tumours, Brain Tumours, Hippocampus, Lung Tumours, Prostate, Cardiac, Pancreas Tumour, Colon Cancer, Hepatic Vessels and Spleen. The data-sets that we have used in the experiments are Spleen and Cardiac data-sets . Both the data-sets have images and their corresponding labels as depth images and volumetric images. Let us look at both the data-sets and their  corresponding properties like range of pixel intensities, number of training 4 and test images and spatial dimensions.
**![](https://lh6.googleusercontent.com/JEW2-HUaDLAKfOIjoqs-zcgYASD3vBSO_kodI7GIkjPMVWkSfJm-CGHgm9BGxdqTCgD9jVV66MXkjF2ExEcaBZaOFZUuYAxfuQnhpF6wpYltnsx9hoMGtMRVJDv64q4nc_XOF67U)**

#### Spleen Data-set
The Spleen dataset contains 41 training images 20 test images with x and y dimensions as 512 and 512 and z(depth) varying from 40-168 roughly in the different training images. The intensities of pixels are ranging from -1024-3072 roughly. All the images in this data-set are gray-scale images.

#### Cardiac Data-set
The cardiac data-set contains 20 training images and 10 testing images with x and y dimensions as 320 and 320 and z(depth) varying from 90-130 in the different training images. The intensities of pixels are ranging from 0-2000 roughly. All the images in this data-set are gray-scale images. The target is left atrium.

#### Results, Conclusions and loss functions used
The Loss functions used, results and  conclusions are explained broadly in the report. An extra work to get a better knowledge of 3D images was done by 3D image clasification using 3D convolution encoder like that on in 3D-Unet/SegNet. The data-set used is 3D MNIST[(link)](https://www.kaggle.com/daavoo/3d-mnist).



[1] Amber L Simpson, Michela Antonelli, Spyridon Bakas, Michel Bilello,Keyvan Farahani,Bram van Ginneken, Annette Kopp-Schneider, Bennett A Landman, Geert Litjens, Bjoern Menze, et al. A large annotated medical image dataset for the development and evaluation of segmentation algorithms. arXiv preprint arXiv:1902.09063, 2019.  <br />
[2]Çiçek, Özgün, et al. "3D U-Net: learning dense volumetric segmentation from sparse annotation." International conference on medical image computing and computer-assisted intervention. Springer, Cham, 2016.
