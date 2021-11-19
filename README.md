# Single Shot Detector

This is the Keras implementation of Single Shot Detector: Towards Real Time Object Detection

### **Note:**

- Only tensorflow backend is supported and this requires tensorflow version 1.x
- Python- 3.7, Keras-2.2.4, CUDA-10.2 versions are used.


## Usage:

### **Training:**
- [ssd512_training](ssd512_training.ipynb) is used to train the model

- The model outputs the following:
   - Model weights in hdf5 format 
   - A CSV file containing all the training metrics
   - Full model image for better understanding of the model architecture

**Note:**
- Input image size is set to 512x512 pixels.
- Pre-trained weights for ResNet can be downloaded from [here](https://github.com/fchollet/deep-learning-models/releases/tag/v0.2)


### **Testing:**
- [ssd512_inference](ssd512_inference.ipynb) is used to test the model

- The test file outputs the following:
   -	Text files for each image with predicted bounding box coordinates, confidence score and its class (saved to a folder)
   -	Test images with bounding box predictions (saved to a folder)

### **Evaluation:**
- [ssd512_evaluation](ssd512_evaluation.ipynb) is used for evaluating the model

- The evaluation file outputs the following:
   -	Prints the Mean Average Precision score
   -	An image of Precison-Recall curve


## API Reference: 
https://github.com/tensorflow/models/tree/master/research/object_detection

## References 
- Implementation adopted from [here](https://github.com/pierluigiferrari/ssd_keras) and is based on the idea of tensorflow’s object detection [API](https://github.com/tensorflow/models/tree/master/research/object_detection).
