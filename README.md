# Object-Detection-Playground
Implementing the fundamentals of Object Detection

### Requirements:
* python3
* keras
* numpy V1.19.2
* scikit-image V0.17.2
* opencv-python
* matplotlib V3.2.2
* tensorflow

### The Object Detection Pipeline:
To build a classic object detection paradigms, there are four key components:
1. **Sliding Window** sits on top of our image and slides from left-to-right and top-to-bottom, classifying each ROI along the way.
2. **Image Pyramid** sequentially reduces the size of our input image. Our sliding window runs on each scale of the image pyramid, enabling us to detect objects that are both closer and farther away from the camera.
3. **Non-maxima Suppression**, when multiple detections surrounding the same object happens after sliding window and image pyramid, it keeps only the most confident prediction.
4. **Batch-processing** ensures our object detector runs as fast possible, especially if a GPU is available.

### Sample outputs of the Object Detection:
![puppy](/output/puppy.PNG)
![horses](/output/horses.PNG)

### References:
* Deep Learning for Computer Vision with Python VOL2 by Dr.Adrian Rosebrock
