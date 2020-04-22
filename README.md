Project 02: Biomedical Image Analysis
============================================================

Supervisor: 

* PD Dr. Karl Rohr (k.rohr@uni-heidelberg.de)
* Christian Ritter (christian.ritter@bioquant.uni-heidelberg.de)
* Roman Spilger (roman.spilger@bioquant.uni-heidelberg.de)
* Leonid Kostrykin (leonid.kostrykin@bioquant.uni-heidelberg.de)
* Svenja Reith (svenja.reith@bioquant.uni-heidelberg.de)
* Qi Gao (qi.gao@bioquant.uni-heidelberg.de)




## Introduction

Image analysis methods are important to extract relevant information from biomedical image data.
Typically a large amount of data needs to be analyzed to draw statistically significant conclusions.
Manual analysis of the image data is tedious, time-consuming, and subjective.
Thus, computer-based image analysis is needed, which enables fast, reproducible, and accurate automated analysis of the data.

To extract information from the image data, methods for different image analysis tasks are required. Typical tasks are image preprocessing, feature extraction, segmentation, object recognition, tracking, and image registration. The projects within the topic "Image Analysis" deal with different image analysis tasks using different methods and different image modalities. The image analysis methods will be implemented in Python using existing libraries (e.g., NumPy, Scikit-learn). 


## Objective

#### Human Face Recognition
The objective of projects 1 and 2 is to implement and evaluate statistical methods for human face recognition (K-nearest neighbors, linear discriminant analysis). For both projects, the first step consists of computing statistical measures for performing data normalization. Second, data dimension reduction should be performed by principal component analysis (PCA) and the results should be visualized. Third, the data set should be split into training and test data sets in order to perform human face recognition.   

* Project 1: Implementation and evaluation of K-nearest neighbors (KNN) algorithm. 
* Project 2: Implementation and evaluation of linear discriminant analysis (LDA). 

#### Cell Nuclei Segmentation
The objective of projects 3 and 4 is to implement and evaluate methods for segmentation of cell nuclei (region growing, clustering). First, a popular evaluation measure known as "Dice score" should be implemented and tested using synthetically generated images. Second, an image segmentation method should be implemented. The methods should be applied to cell nuclei images and the average Dice score should be computed. Third, pre-processing methods such as Gaussian filtering should be investigated to improve the result.

* Project 3: Implementation and evaluation of region growing.
* Project 4: Implementation and evaluation of clustering method.

#### Biomedical Image Registration
The objective of project 5 is to implement and evaluate feature-based image registration methods using a similarity transformation. First, corresponding points (>20) should be manually annotated in each pair of images to be registered. Second, two pairs of corresponding points should be chosen and the transformation parameters (translation, rotation, scaling) should be determined (Method 1). Third, images should be transformed using inverse mapping (inverse warping) and bilinear interpolation, and the registration accuracy should be evaluated using suitable performance measures. Fourth, 10 (or more) pairs of corresponding points should be chosen to compute the transformation parameters based on a least-squares method (Method 2), and the registration accuracy should be evaluated and compared with Method 1.

* Project 5: Implementation and evaluation of feature-based image registration.


## Description of datasets

#### Human Face Recognition
The Yale Face Database of human faces consists of 165 images from 15 subjects. Per subject exist 11 images with the following facial expressions or configurations: center-light, with glasses, happy, left-light, without glasses, normal, right-light, sad, sleepy, surprised, and wink. The images are grayscale images normalized by size (320×243 pixels) and stored as GIF files. 

#### Cell Nuclei Segmentation
The dataset for cell nuclei segmentation consists of 25 images of bone-marrow derived macrophages from mice from the Broad Bioimage Benchmark Collection. The cell nuclei were stained with DAPI. The images have a size of 1388×1040 pixels and show 30–50 cell nuclei per image. 

#### Biomedical Image Registration
The dataset for image registration consists of two pairs of images. The first pair (cameraman) contains two natural images. The second pair (cells) contains a fluorescence and a bright field microscopy image.
For both image pairs, the images denoted as moving need to be transformed towards the reference images denoted as fixed.


## Literature 

#### Human Face Recognition
* Gerbrands, J.J. "On the relationships between SVD, KLT and PCA." Pattern Recognition (1981), vol. 14, issues 1-6, pp 375-381
* Belhumeur, P.N., Hespanha, J.P. and Kriegman, D. "Eigenfaces vs. Fisherfaces: Recognition Using Class Specific Linear Projection." IEEE Transactions on Pattern Analysis and Machine Intelligence (1997), vol. 19, pp 711-720.
* Gareth, J. and et al. "An introduction to statistical learning." Springer New York (2013), Chapter: 4.4

#### Cell Nuclei Segmentation
* Ljosa, V., Sokolnicki, K.L. and Carpenter, A.E. "Annotated high-throughput microscopy image sets for validation." Nature Methods 9.7 (2012), pp 637-637.
* Shih F.Y. and Cheng S. "Automatic seeded region growing for color image segmentation." Image and Vision Computing (2005), vol. 23, issue 10, pp 877-886
* Szénási S. "Distributed region growing algorithm for medical image segmentation." International Journal of Circuits, Systems and Signal Processing (2014), vol. 8, pp 173-181
* Lin, Z., Jin ,J.S. and Talbot, H. "Unseeded region growing for 3D image segmentation." Proceedings of the Pan-Sydney Area Workshop on Visual Information Processing (2000), vol. 2, pp 31-37

#### Biomedical Image Registration
* Szeliski, R. “Computer Vision: Algorithms and Applications”. Springer (2011). Sections 3.6.1 and 6.1.1. (see http://link.springer.com/openurl?genre=book&isbn=978-1-84882-935-0)
* http://www.comp.nus.edu.sg/~cs4243/lecture/register.pdf


## How to structure your project

### Project proposal

For all projects within the topic "Image Analysis" the first task 
is to define a **project proposal**, which should include

* List of planned analysis steps
* Milestones (important achievements)
* Deliverables (result for each milestone)
* Approximate timetable

The project proposal will be presented three weeks after the beginning of the semester (10 min presentation + 5 min discussion). 








