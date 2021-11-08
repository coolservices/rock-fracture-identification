# Rock-Fracture-Identification

## Description

In 2017, Chaurasia et al proposed LinkNet network model (Patel et al., 2015). D-LinkNet is a neural network model for image semantic segmentation, which is improved on the basis of the LinkNet network model by adding the dilated convolution module and Resnet module suitable for small target semantic segmentation. D-LinkNet was once used in the field of satellite road identification. We made some improvements, such as adjusting the convolution pooling depth and the loss function, in order to be better applied to the semantic segmentation of rock fractures.

## Application Environment

Applying the computer programming language Python on Linux systems.

## Usage

We segmented the collected rock fracture images and trained them in the D-LinkNet model using the cross-training method. We set the ratio of training set: validation set = 9:1. We need to set the input image size, learning rate, batch size and other parameters according to the difference of data sets.

A reasonable set of input parameters are as follows:

```python
trainimg = 'data/New1/Train yuan new 1'
trainseg = 'data/New1/Train new seg'
valimg = 'data/New1/val yuan new 1'
valseg = 'data/New1/Val new seg'
epochs=40
batchsize = 2
val_batchsize = 2
learningrate = 0.00005
width = 512
height = 512
weightdecay = 1e-8
n_channels = 3
n_class = 1
modelname = 'DeepLab'
```



## Related Publications

Gu, Q.H., 2020. Road Intelligent Identification and Road Network Modeling of Open Pit Mine based on D-LinkNet Network. Journal of China Coal Society 45(S2), 1100-1108 [in Chinese]. https://doi.org/10.13225/j.cnki.jccs.2020.0414.

Patel, D., Hsu, W., Lee, M.L., 2015. LinkNet: capturing temporal dependencies among spatial regions. Distrib Parallel Dat 33, 165-200. https://doi.org/10.1007/s10619-014-7147-9.

Xu, H., Su, X., Wang, Y., Cai, H., Cui, K., Chen, X., 2019. Automatic Bridge Crack Detection Using a Convolutional Neural Network. Applied Sciences 9, 2867. https://doi.org/10.3390/app9142867.

Xue, D.J., Tang, Q.C., Wang, A., Zhang, L., Zhou, H.W., 2019. FCN-based intelligent identification of crack geometry in rock or concrete. Chinese Journal of Rock Mechanics and Engineering 38, 3393-3403 [in Chinese]. https://doi.org/10.13722/j.cnki.jrme.2019.0010.

## Major project leaders and their contributions

D.D. Pan contributed in the developed of idea, design Network. 

Y.H. Li obtained the input data, developed and tested the code and analyzed the results.

Z.H. Xu obtained the input data and contributed in the code.

## Acknowledgements

We would like to appreciate the financial support from the National Science Fund for Excellent Young Scholars (Grant No.: 52022053), the Science Fund for Distinguished Young Scholars of Shandong Province (Grant No.: ZR201910270116), and the China Postdoctoral Science Foundation (Grand No. s: BX2021172; 2021M691953).

## License

Rock-Fracture-Identification is licensed under the [Apache License 2.0](https://github.com/zsylvester/meanderpy/blob/master/LICENSE.txt).