# Style-Recognition-
recognizing styles of painitngs of different artists through residual neural networks

# Neural networks architecture
RESNET:
The ResNet has input dimensions of 224×224×3.Its architecture is composed of different blocks,  where each block uses a ”shortcut connection”.  This shortcut connection can be a simple identity connection (id-block), or a connection with a convolutional layer (conv-block).  The shortcut-ed part of the block uses 3 convolutions, with various number of filters for each block.  The first and third convolution of this group use filters sizes of 1 x 1, and the second one is usually 3 x 3.  At the end of a block, the features of the shorcut part and the shortcut-ed part are added.  Each convolutional layer is followed by a batch-normalization
layer.

The ResNet50 starts with a  convolutional  layer  with  a  filter  size  of  7x7,  generating  64  filters,  followed  by  a  batch-normalization layer, an activation layer and a max-pooling layer.  Then there are 4 groups of blocks, each starting with a conv-block(3 convolutional layers).  Each group contains respectively 1, 3, 5 and 2 id-blocks.  The ResNet50 contains in total 53 (3 +(1+3+5+2)) convolutional layers. 
