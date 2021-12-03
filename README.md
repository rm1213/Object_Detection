# Object_Detection

For the task of object detection i.e. cars and people from images, the following approach has been used:
1. Model Selection – The deep learning model used for the task of object detection is Mask R-CNN. Mask R-CNN is a Convolutional Neural Network (CNN) and state-of-the-art in terms of image segmentation. This variant of a Deep Neural Network detects objects in an image and generates a high-quality segmentation mask for each instance. Mask R-CNN is an extension of Faster R-CNN and works by adding a branch for predicting an object mask (Region of Interest) in parallel with the existing branch for bounding box recognition. 
The model used in our case is a pretrained model on COCO Dataset. 
2. Choice of Dataset – In our case, the model has been a pretrained model on COCO dataset. The MS COCO (Microsoft Common Objects in Context) dataset is a large-scale object detection, segmentation, key-point detection, and captioning dataset.  
The COCO dataset was extracted via COCO API which provides support for Python, MATLAB and other languages. Since, the overall task had been done in Python, it became convenient to use COCO API for reading data.
Since, different types of objects ranging from airplane, person, bicycle, car etc. could be easily identified using COCO dataset, it fulfilled our objective to identify the two classes i.e. person and cars in the images. 
3. Evaluation metrics – The evaluation metrics consist of average precision for loss function, IOU (Intersection over Union) scores as well as confidence score returned by Mask-RCNN. The confidence score defines the probability or confidence for each predicted class. Bounding boxes are drawn around objects detected which have confidence score higher than a defined threshold. 
