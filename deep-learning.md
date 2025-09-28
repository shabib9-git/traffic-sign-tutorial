[Home](index.md) | [Classical](classical.md) | [Deep Learning](deep-learning.md) | [Datasets & Eval](datasets.md) | [Success/Failure](successes-failures.md) | [Challenges](challenges.md) | [Future](future.md) | [Refs](bibliography.md)

# Deep Learning

Deep learning has transformed traffic sign detection and classification by learning features directly from data, rather than relying on hand-crafted descriptors.

## CNN-based classification
Convolutional Neural Networks (CNNs) learn hierarchical features (edges → shapes → symbols) from sign crops and achieve high accuracy on benchmarks.

![CNN Architecture](assets/images/cnn-architecture.png)  
*Figure: Simplified CNN architecture for sign classification.*

## Real-time detection on device
Lightweight detectors (e.g., MobileNet variants and YOLO-tiny) can localize and classify signs in full images at real-time rates on mobile/embedded hardware.

![YOLO Detection](assets/images/yolo-detection.png)  
*Figure: YOLO-style detection mockup with bounding boxes.*

## Emerging approaches
Transformer-based models and hybrid CNN–Transformer backbones improve robustness for **small** or **partially occluded** signs by modeling long-range context.  
Quantization/pruning and TensorFlow Lite/NNAPI help deploy models efficiently on phones.

<audio controls src="assets/audio/deep.mp3">Your browser does not support audio.</audio>
