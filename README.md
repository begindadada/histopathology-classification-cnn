# histopathology-classification-cnn
 Categorization of histopathological images using different pre-trained convolutional neural networks


	This thesis has as a main subject the categorization of Histopathological Images, using various models of Convolutional Neural Networks (CNN).
 The purpose of this study was to examine the use of machine learning and, specifically, deep learning approaches, 
 in the automatic categorization (classification) of medical images. The classification procedures are tested based on deep neural networks (DNN) and,
 specifically, Convolutional Neural Networks. Today, these networks belong to the scientific field of pattern recognition, 
 constituting the state-of-the-art and they are techniques for classifying images of medical databases. CNNs exist in different architectures, 
 with different depth, multitude of convolutions, activation functions and many other parameters and technologies. 
 In the present work we examined architectures that exhibit distinctive behavior in the classification of medical data.
 From these we selected eight CNN which we tested during the experimental process: Vgg16, Vgg19, ResNet50, ResNet101, ResNet152, MobileNet, MobileNetV2 and DenseNet121.
 For training and testing the systems, histopathological images of breast cancer were used as medical data, 
 which were classified into positive (malignant) and negative (benign), for tumor recognition. Specifically, 
 the Histopathological Database Breast Cancer (BreaKHis) was used, containing 7,909 images, collected from 82 patients: 58 with cancer (5,429 malignancies) and 24 
 with benign neoplasms (2,480 benign). Image resolution is 700x460 pixels, RGB 3 channels, 8-bit depth. 
 The images in the database are divided (approximately equally), depending on the magnification of the microscope into four categories: 
 40x, 100x, 200x and 400x. Note that all CNNs we used were initially trained (pre-trained), 
 in the vast amount data of ImageNet database. These eight networks were trained and tested in three experimental procedures: 
 one without pre-process, one with ZCA pre-preprocess, and one with PCA. Finally, all experiments were repeated four times, 
 corresponding to the different categories of focus data (40x, 100x, 200x, 400x). 
 Thus, the total number of experiments carried out was 96 experiments, and the results are posted in 31 confusion matrices and 8 figures. 
 The eight networks that we tested were compared with each other and we easily came to the conclusion that DenseNet121 network has the best performance.
 It was expected, as this is an evolution of the ResNet networks. It was also interesting to note that low-focus images performed better results, than high-focus images.
 In the experiments, where the data had been previously preprocessed, with the ZCA technique and the PCA, the results could not be characterized as expected.
 The pre-processed based on the ZCA technique gave slightly better results than that of the PCA.
 However, comparing these two approaches with the non-pre-processed approach, we found a clear superiority without pre-processed. 
 The explanation we can give for these results is that the limited volume of training and testing data did not allow the contribution of the preprocessing stage to emerge.