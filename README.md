Assignment - 1(Data Preparation and Understanding)
Data Preparation and Understanding 
XML Processing, Image Cropping and Resizing, and Histogram Comparison
Project Overview :
This project involves XML processing, image cropping and resizing, and various image processing techniques using scikit-image. The main functionalities include converting normal images to grayscale, plotting grayscale images with their corresponding pixel intensity histograms, applying the Sobel edge filter, calculating edge histograms, and performing histogram comparison using different metrics. Additionally, Histogram of Oriented Gradient (HOG) feature descriptor and dimensionality reduction using Principal Component Analysis (PCA) are implemented.
Processing XML
The project initiates, by processing XML to extract data from XML files. The `xml_processor.py` module handles the parsing of XML files extracting information and preparing it for image processing.
Image Manipulation
Cropping and Resizing Images
In the `image_processor.py` module there are functions for manipulating images. These functions allow for cropping and resizing images to a dimension ensuring uniformity in input data for processing steps.
Conversion to Grayscale
Images are converted to grayscale using scikit image library simplifying the color information and enhancing processing efficiency. Grayscale images are known to capture features required for image analysis tasks.
Sobel Edge Filtering
The Sobel edge filter is applied to grayscale images in order to highlight edges and contours. This process provides information about the structure and boundaries within the images.
Calculation of Edge Histograms
Edge histograms are computed for each image capturing the distribution of edge intensities. These histograms serve as features that can be further analyzed and compared.
Comparison of Histograms
Within the `histogram_comparison.py` module three distinct metrics are utilized for histogram comparison;
1. Euclidean Distance; This metric measures the straight line distance between two points in a space. In terms of histogram comparison it provides a measure of dissimilarity, between two histograms.
Calculating the Manhattan distance, known as L1 norm or city block distance involves summing the differences, between corresponding values in two histograms. This approach offers a perspective on measuring dissimilarity between histograms.
The cosine distance measures the cosine of the angle between two histograms treating them as vectors in a dimensional space. It provides a measure of similarity that is normalized by the magnitude of the histograms.
To compute Histogram of Oriented Gradient (HOG) features for each image you can utilize the `hog_descriptor.py` module. HOG is a technique used for object detection and image recognition capturing information, about gradient orientation distribution.
When dealing with data efficiently while preserving crucial information it's essential to apply Principal Component Analysis (PCA) for dimensionality reduction. The `pca_reduction.py` module can assist with this step.
All processed images, histograms and comparison results are conveniently stored within the `results/` directory.
Visual representations, like plots and output images play a role in helping users grasp the effects of processing steps on input images.
Prerequisites :
Ensure you have the following dependencies installed before running the project:
- Python (>= 3.6)
- scikit-image
- NumPy
- Matplotlib
-PYCharm
You can install these dependencies using the following:
pip install scikit-image numpy matplotlib
PYCharm installation can be done here: https://www.jetbrains.com/pycharm/
Usage:
1. Clone the repository:
git clone https://github.com/yourusername/yourproject.git
cd project
2. Run the main script:
python main.py
The script will execute the entire pipeline, including XML processing, image manipulation, and histogram comparisons.
Project Structure:
 - `data/`: Contains XML files and input images.
 - `src/`: Holds the source code files.
  - `xml_processor.py`: Handles XML processing.
  - `image_processor.py`: Contains functions for image cropping, resizing, grayscale conversion, Sobel edge filter, and edge histogram calculation.
  - `histogram_comparison.py`: Implements histogram comparison using Euclidean distance, Manhattan distance, and Cosine distance.
  - `hog_descriptor.py`: Computes Histogram of Oriented Gradient (HOG) features.
  - `pca_reduction.py`: Applies Principal Component Analysis (PCA) for dimensionality reduction.
  - `main.py`: The main script that integrates all modules and performs the complete image processing pipeline.
- `results`: Stores the output images and plots generated during the process.
Acknowledgments:
- The project relies on the scikit-image library for image processing tasks.
- Various image processing techniques are applied based on scikit-image documentation and examples.
- Python is used in this project because of its platform independency feature.
- This project heavily relies on the scikit image library, which provides robust capabilities, for image   processing.
 - To implement different image processing techniques we referred to the documentation and examples provided by the scikit image library.
License :
This project is licensed under the MIT License -1
System requirements :
Optimal performance on windows 10 and 11.
Recommended operating systems: windows 9 and above, Linux and mac
Required Storage: 1GB and above.




