# My Recognition

This project is a simple image classification script using NVIDIA Jetson's `jetson-inference` and `jetson-utils` libraries. It allows you to classify images using pre-trained models like GoogLeNet or ResNet-18.

## Example Output image is recognized as Labrador retriever (class #208) with 98.23% confidence##  Requirements

- Jetson Nano (or other Jetson device)
- Ubuntu 18.04+
- NVIDIA JetPack SDK installed
- [jetson-inference](https://github.com/dusty-nv/jetson-inference) library built and installedmy-recognition/
├── my-recognition.py # Main classification script
├── dog_0.jpg # Sample image
├── orange_0.jpg # Sample image
├── polar_bear.jpg # Sample image##  How to Run
1. **Navigate to the project folder:**

cd ~/my-recognition
Run the Python script:

python3 my-recognition.py --filename your_image.jpg
Replace your_image.jpg with the path to your test image.

Optional: Use a different network model

python3 my-recognition.py --filename your_image.jpg --network=resnet-18
Supported Networks:
googlenet (default)

resnet-18

alexnet

squeezenet

others supported by jetson-inference

## Customize It
Add more images to test.

Replace the classification model with a custom one using transfer learning.

Extend the script to classify live webcam input or video.

## Resources
Jetson Inference GitHub

NVIDIA Jetson AI Courses
iD Tech NVIDIA Jetson AI Course
## Author
McCatNaps (Jetson Nano)
