# SparseTorch

Protyping and development repo here. 
https://github.com/Santosh-Gupta/Prototyping


Sparse Pytorch Training Library 

Biggest hurdle: latency of reading/writing values to memory mapped files. 

To do:

-test data gadget

-See if you can speed up regular pytorch wordvec with pytorch cpu pinned. Or maybe in just gpu. 

-Look into cupy memmapes to start data. the cpu pinned one. test on pytorch word2vec. Store the `data` array as a .npy file. Convert to int64 before you do. 
then open in in cpu mounted cupy arrays. probably have use dlpack to extract tensors to feed into pytorch embedding lookup. Then benchmark against the pinned pytorch cpu arrays. 

---------

-Fastest way to retrieve/write hundreds of thousands of float32 arrays in an instance, and set them to Pytorch tensor. 

Investigate parallelization, during machine learning forward pass/backwards pass/weight update. 

Maximize use of CPU + GPU ram. Optimal pre-fetching and parallelization depending on training parameters. 

What is it. 
