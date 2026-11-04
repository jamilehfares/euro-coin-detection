# Euro Coin Detection and Classification

## Project Overview
This project aims to develop an automatic coin detection system that identifies euro coins in images and calculates their total monetary value. The system utilizes computer vision techniques, specifically the Hough Transform for circle detection, and a neural network for classification of the detected coins.

## Objectives
- Detect euro coins in images by identifying circular edges.
- Classify the detected coins based on their radii.
- Optionally train a neural network to improve classification performance.
- Calculate the total monetary value of all detected coins.

## Methodology
1. **Image Loading**: The project begins by loading images containing euro coins from a specified directory.
2. **Preprocessing**: Images are resized to reduce computational cost and improve processing speed.
3. **Coin Detection**: The Hough Transform is applied to detect circular shapes in the images, which correspond to the coins.
4. **Classification**: Detected coins are classified based on their radii using predefined thresholds. Additionally, a neural network is trained to enhance classification accuracy, especially for coins with similar sizes.
5. **Monetary Calculation**: The total value of the detected coins is calculated and displayed.

## Results
The system has been tested on various images containing euro coins. The results indicate that while the Hough Transform effectively detects coins, challenges remain in distinguishing between coins of similar sizes, such as the 50-cent and 1-euro coins. The integration of a neural network has shown promise in improving classification accuracy.

## Future Work
To enhance the performance of the coin detection and classification system, future work may include:
- Expanding the dataset to include more diverse images of coins.
- Improving the neural network architecture for better classification results.
- Implementing additional preprocessing techniques to handle varying lighting conditions and occlusions.

## Installation
To run this project, ensure you have the following libraries installed:
- OpenCV
- NumPy
- Matplotlib
- PyTorch
- torchvision

You can install the required libraries using pip:
```
pip install opencv-python numpy matplotlib torch torchvision
```

## Usage
Run the Jupyter Notebook located in the `main` directory to execute the coin detection and classification process. Follow the instructions within the notebook for loading images and viewing results.