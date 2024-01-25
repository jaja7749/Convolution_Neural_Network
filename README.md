# Convolution Neural Network

## Data, parameter and shape:

1. let's definite some parameter:
   - $`c`$ : channels (in_channels)
   - $`k`$ : kernels (out_channels)
   - $`s`$ : stride
   - $`p`$ : padding

2. determine the data shape:
   - $`Z\in \mathbb{R}^{k\times i\times j}`$ : output data (shape: out_channels, col, row)
   - $`A\in \mathbb{R}^{c\times k\times l}`$ : input data (shape: in_channels, col, row)
   - $`\omega \in \mathbb{R}^{k\times c\times m\times n}`$ : weight (shape: in_channels, out_channels, kernel_size, kernel_size)
   - $`b\in \mathbb{R}^{k}`$ : bias (shape: out_channels)

3. calculate the output shape:
   - $`i=\frac{k-m+2p}{s}+1`$
   - $`j=\frac{l-n+2p}{s}+1`$

## Convolution layer:


