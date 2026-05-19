# JPEG-2000-Wavelets-Paper
A school project investigating the wavelets used in the JPEG 2000 Wavelets. Produced in collaboration with Benjamin Langford

In an increasingly digital age, where data usage and storage are at an all-time
high, efficient compression standards are essential. With modern personal com-
puters storing upwards of a terabyte of data and large data centers exceeding
several exabytes of storage1, it is necessary to have a standardized file format
that increases data portability and reduces file size. The JPEG2000 standard
aims to do that. Improving upon its predecessor, JPEG, JPEG2000 introduces a
different method for both lossless and lossy image compression. While the older
standard utilized discrete cosine transforms (DCTs) to convert small blocks of
pixels into the frequency domain, the JPEG2000 standard uses discrete wavelet
transforms (DWTs) and multi-resolution analysis.
Instead of using a Fourier-based method to retrieve different levels of detail
in an image, JPEG2000 implements two different wavelets that allow for the
filtering of an image based on one’s needs, lossy or lossless compression. The
first wavelet, used for lossy compression (a type of compression in which data
is discarded to reduce file size), is known as the Cohen-Daubechies-Feauveau
9/7 wavelet or 9/7 Daubechies for short. The second wavelet, used for lossless
compression (a type of compression in which the original data is retained to
maintain image quality), is known as the LeGall-Tabatabai 5/3 wavelet or 5/3
LeGall for short.
The topic of this paper is centered around these two wavelets, 9/7 Daubechies
and the 5/3 LeGall. In section 2, the paper will discuss basic properties of these
two wavelets and why they are important. It will cover the biorthogonality
property, vanishing moments, and the lifting scheme. Section 3 of the paper
will discuss the unique properties of the 9/7 Daubechies wavelet and why this
particular wavelet is well-suited to the application of image compression. Section
4 will similarly discuss the 5/3 LeGall wavelet with the addition of its natural
coefficients. Section 5 will demonstrate how the wavelets are used in the context
of the JPEG2000 standard. A simple example will be given after explaining the
background of how and why images are first encoded. Finally, section 6 will
conclude this paper and offer closing remarks.
