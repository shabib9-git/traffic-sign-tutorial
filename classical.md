[Home](index.md) | [Classical](classical.md) | [Deep Learning](deep-learning.md) | [Datasets & Eval](datasets.md) | [Success/Failure](successes-failures.md) | [Challenges](challenges.md) | [Future](future.md) | [Refs](bibliography.md)

# Classical Detection Methods

This page covers simple, classical approaches before deep learning.

## Color-based approaches
- Many traffic signs use strong colors like red borders or yellow backgrounds.  
- Thresholding these colors helps isolate likely regions.  
- Morphological operations can clean up the masks.  

![Stop Sign](assets/images/stop.jpg)  
*Figure: STOP sign example.*

## Shape-based approaches
- Signs use standardized shapes: circles, triangles, octagons.  
- The Hough transform and contour analysis can identify these shapes.  

![Hough Example](assets/images/hough-example.png)  
*Figure: Hough transform detecting circles.*

## Handcrafted features (HOG + SVM)
- Histogram of Oriented Gradients (HOG) captures edge directions.  
- SVM classifiers can then distinguish sign types based on these features.  

These methods are simple and effective in controlled conditions, but they often fail in complex, real-world environments where lighting, occlusion, or blur are present.

<audio controls src="assets/audio/classical.mp3">Your browser does not support audio.</audio>
