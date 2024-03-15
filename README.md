# Face Recognition System using Eigenfaces

A face recognition system using algorithm called Eigenface and a benchmarking system to evaluate how accurate the system is in recognizing the faces according to the given dataset

## Features

This system can detect faces by treating the face recognition problem as a 2-D recognition problem. 
We project the set images into a face space known as eigenfaces. Eigenfaces is an algorithm that uses principal component analysis (PCA) to analyze face images and identify patterns (based on ears, eyes, mouth, nose) that represents a face.
There are mainly 3 components in this system
#### 1) Image I/O and Visualization 
#### 2) PCA for training 
#### 3) Recognition by Nearest Neighbor classification.

## MATLAB Usage

I used MATLAB for implementing the face recognition model, training, and testing. MATLAB is a high-level programming language and environment for numerical computation, visualization, and programming. Learn more about MATLAB from the [official MATLAB website](https://www.mathworks.com/products/matlab.html).

## Example Dataset
I considered 32 X 32 8bit images (Nx by Ny) (.TIF files)
There are 3 Folders
- [FA](#Image dataset for Training)
- [FB](#Image dataset for testing)
- [ALL](#FA + FB)

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/hackerdud3/Face-Recognition-Eigenfaces.git

2. Change the folder path for ALL, training dataset(FA), and testing dataset(FB).
   ```sh
   % Path to training set
   path = "\ALL";
   % Construct DB from this dataset
   path = "\FA";
    % Path to testing set
   path = "\FB";
   
   

