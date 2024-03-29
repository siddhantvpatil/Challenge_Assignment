# VMG_Challenge_Assignment
The repository contains PyTorch implementation of "BioFaceNet: Deep Biophysical Face Image Interpretation". The current status of this repo is work in progress.

**Link to Article:** https://arxiv.org/abs/1908.10578

**Requirements:**
Python3,
PyTorch,
NumPy,
Pandas,
Matplotlib

**Pre-defined values:**
The matrices required for computation are uploaded in the utils folder. Update the "folder_path" in the cell "Python Code for setup.m" to point to the matrices in util folder.

**Dataset:**
CelebA dataset is used for training, validating and testing the pipeline. The dataset can be downloaded from http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html 

The code is in the form of a Jupyter notebook. Please run all the cells sequentially. Assign the path to the input image folder to the variable "data_root". 

**Note:**
* The entire pipeline is not functional. The loss computation and backward propagation need an update.
* The dimensions provided in the comments of the functions are with respect to [Matlab implementation](https://github.com/ssma502/BioFaces). The same can be used for doing a first pass on the implementation of the functions in Python. In general, Matlab uses the dimensions as (Height x Width x Number of channels x Batch Size) and PyTorch refers to (Batch Size x Number of channels x Height x Width). Also, while comparing the Python and Matlab implementation, do note that indices in Python start with 0 and in Matlab, they start with 1.
