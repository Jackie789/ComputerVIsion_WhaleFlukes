# ComputerVIsion_WhaleFlukes
We seek to differentiate whale individuals by the patterning on their flukes. 

This dataset has been downloaded from a Kaggle Dataset, which can be found [here]  (https://www.kaggle.com/c/whale-categorization-playground). 


![Example Whale Fluke]  (https://github.com/Jackie789/ComputerVIsion_WhaleFlukes/blob/master/assets/0ae14ed7.jpg "Example Whale Fluke Image")

## Introduction

The coloration on a whale's tail is unique to each individual, similar to a fingerprint on a human. 

In this dataset, we have 4,251 unique humpback whales, with 52.2% of the whale individuals only photographed one time. Another 8.2% of the dataset are unknown, "new" whales. 

Some whales are more common in the dataset, appearing up to 34 times. 

The dataset is somewhat messy. Some photographs are in color, others are black and white. Some of the photographs are annotated with the whale id#, some are zoomed out, although the biggest challenge of this dataset will be artifically growing the dataset for the under-represented individuals. 

## Approach

Let's use a combination of zoom, tilt, and stretching techniques to artificially help oversample the under-represented individuals in the dataset. We use a computer vision package **conx**, which sits on top of TensorFlow and Keras, to build our neural networks. 

