# Object Detection | FasterRCNN
This repository uses torchvision's Faster R-CNN implementation which has been shown to work well on a wide variety of Computer Vision problems.
For the DetectionLearner, we use Faster R-CNN as the default model, and Stochastic Gradient Descent as our default optimizer.
Our Faster R-CNN model is pretrained on COCO, a large-scale object detection, segmentation, and captioning dataset that contains over 200K labeled images with over 80 label categories.

## Data
In this notebook, we use a toy dataset called Fridge Objects, which consists of 134 images of 4 classes of beverage container {can, carton, milk bottle, water bottle} photos taken on different backgrounds.

You'll notice that we have two different folders inside:

* /images
* /annotations

This format for object detection is fairly common.

/data

+-- images

|   +-- image1.jpg

|   +-- image2.jpg

|   +-- ...

+-- annotations

|   +-- image1.xml

|   +-- image2.xml

|   +-- ...

+-- ...

Each image corresponds to an xml file. Each xml file contains information on where its corresponding image file is located. It also contains information about the bounding boxes and the object labels. In this example, our fridge object dataset is annotated in Pascal VOC format. This is one of the most common formats for labelling object detection datasets.

## Output
![](/det_output.jpg)
