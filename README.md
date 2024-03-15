# Face Recognition System using Eigenfaces

A face recognition system using algorithm called Eigenface and a benchmarking system to evaluate how accurate the system is in recognizing the faces according to the given dataset

## Features

This system can detect faces by treating the face recognition problem as a 2-D recognition problem. 
We project the set images into a face space known as eigenfaces. Eigenfaces is an algorithm that uses principal component analysis (PCA) to analyze face images and identify patterns (based on ears, eyes, mouth, nose) that represents a face. I also plotted cummulative distribution between the eigenvalues and eigenvectors.
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

2. Change the folder path for ALL, training dataset(FA), and testing dataset(FB):
   ```sh
   % Path to training set
   path = "\ALL";
   % Construct DB from this dataset
   path = "\FA";
   % Path to testing set
   path = "\FB";

3. Manually change the K value for selecting the top K eigenvector:
   ```sh
   %top K eigenvectors 
   k = 10
Try testing out the accuracy with different inputs of K values.

4. Run the MATLAB script file (.m) from the MATLAB command line window:
   ```sh
   >>EigenFaces

## Snapshots
#### Accurate matches

<img width="842" alt="Screenshot 2024-03-13 203120" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/cb95ba2a-fe91-4627-a73e-5d23af9f7d2f">
<img width="838" alt="Screenshot 2024-03-13 202934" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/9a9a6e57-999d-4816-a60d-09f97ed1ca20">
<img width="842" alt="Screenshot 2024-03-13 202917" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/3b835e55-8109-469c-96bc-daeb58b806df">
<img width="820" alt="Screenshot 2024-03-13 202831" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/078a112e-959a-4e7d-abfb-3d413e249720">
<img width="828" alt="Screenshot 2024-03-13 202814" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/049bb051-0b9a-4d3b-828c-5547ec84e64e">
<img width="831" alt="Screenshot 2024-03-13 202750" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/178a6a36-c5ff-489a-817a-a75a504849b4">
<img width="353" alt="Screenshot 2024-03-13 203440" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/a8029ac2-bcfa-4250-b75f-792862ea7aca">

#### Inaccurate matches

<img width="365" alt="mismatch2" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/1aa29381-74d4-495d-b37b-6d3a7148a56a">
<img width="359" alt="mismatch1" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/dbc5a2af-a371-4e1d-97ae-70a6199d2a70">
<img width="356" alt="Screenshot 2024-03-13 203558" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/5e701e1e-d829-4fde-9872-ec96535895b7">

## Plot

<img width="959" alt="Screenshot 2024-03-13 204431" src="https://github.com/hackerdud3/Face-Recognition-Eigenfaces/assets/28582589/f57d259e-7c37-4a20-92a1-a31a6a368c9f">

## Accuracy
Total number of correct matches: 17 
Total number of incorrect matches: 6 
Accuracy : 73.9130 

The accuracy depends on various parameters including value of K, set of training images, and dimensions of the 
images (Nx by Ny), which is resolution. I considered 32 x 32 images here and small training 
se. We can probably improve accuracy if we included more datasets for 
training and considered images with more dimensions.

   

