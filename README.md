# Semantic-Segmentation-of-Aerial-Images
The project utilizes a dataset that contains aerial imagery of Dubai. It is  annotated with pixel-wise semantic segmentation of 6 classes namely buildings,  roads, lands, vegetation, water and lastly unlabeled. The original images and masks are processed separately using various image processing techniques.  
Then the U-net model is defined and fit onto the training data. It is a CNN used for fast and precise segmentation of images. The architecture consists of a contracting path and an expansive path. The contracting path contains encoder layers that capture contextual information and reduce the spatial resolution of the input, while the expansive path contains decoder layers that decode the encoded data and use the information from the contracting path via skip connections to generate a segmentation map. 
Evaluation metrics used are of accuracy and Jaccard index, also known as intersection over union which is used to gauge the similarity between the predicted and actual images. 
Loss function used is focal class which is applies a modulating term to cross entropy loss function in order to focus learning on hard misclassified samples. 
The trained model is used for prediction on the test dataset and sample images are shown. The model achieves an accuracy of nearly 90%. 
 
