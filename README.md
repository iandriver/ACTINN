## Overview
NNICT (Neural Network Identifies Cell Types in scRNA-Seq) is a useful tool to quickly and accurately identify cell types in scRNA-Seq. For details, please read the paper:

## Prerequisite
python 3.6

python packages:
tensorflow 1.10+, numpy 1.14+, pandas 0.23+, argparse 1.1+, scipy 1.1+, scanpy 1.3+

## Usage
We use HDF5 format for the scRNA-Seq expressiong matrix, which stores the compressed matrix and is fast to load. To convert the format, we first read the expression matrix as a pandas dataframe, then we use the to_hdf function to save the file as h5 format. For the to_hdf function, we use "dge", which stands for digital gene expression, for the key parameter.

Here's an example:
'''
python format.py -i input_file -o output_file -f 10X
'''