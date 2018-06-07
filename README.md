# Fluorescence microscopy images

The dataset contains 2661 cell nuclei of 37 fluorescence microscopy images. The cells were taken from the Huh7 and HepG2 liver cancer cell lines and stained with nuclear Hoechst 33258. Their images were digitized at 20x microscope objective lens and pixel resolution was 768×1024. The nuclei in these images were manually annotated by our biologist collaborator.

The images are numbered starting from 1. The first 25 images belong to the cell line, Hepg2. The rest belong to Huh7 cell line. 

We split the dataset into two sets, training and test sets. To have a fair benchmarking, you may want to use the same training and test sets. Below, you can find the images used for training and test sets, seperately.


* Training set: 
    * Hepg2 -> 1, 3, 7, 15, 23
    * Huh7 -> 27, 28, 33, 35, 39
    
* Test set: 
    * Hepg2 -> 2, 4, 5, 6, 11, 12, 13, 14, 16, 17, 18, 19, 20, 21, 24, 25
    * Huh7 -> 26, 29, 30, 31, 32, 34, 36, 37, 38, 40, 41
    
We use 785 nuclei of ten randomly selected images (five Huh7 and five HepG2 cell line images) in the training set, on which the model parameters are estimated. The nuclei in the remaining 27 images are used for testing. HepG2 cells tend to grow in more overlayers than Huh7 cells. This leads to more overlapping nuclei in the images of the HepG2 cell line. Thus, we separately test our algorithm for these cell lines. The Huh7 cell line test set includes 891 nuclei of 11 images and the HepG2 cell line test set includes 985 nuclei of 16 images.

# Publications using the dataset
You can find the publications published by our group which use this dataset for experimental analysis:
```
[1] C.F. Koyuncu, R. Cetin-Atalay, and C. Gunduz-Demir, "Object Oriented Segmentation of Cell Nuclei in Fluorescence
Microscopy Images," Cytometry: Part A (in revision).
[2] C.F. Koyuncu, A. Akhan, T. Ersahin, R. Cetin-Atalay, and C. Gunduz-Demir, "Iterative h-minima based marker-controlled watershed for cell nucleus segmentation," Cytometry: Part A, 89A:338-249, 2016.
[3] S. Arslan, T. Ersahin, R. Cetin-Atalay, and C. Gunduz-Demir, "Attributed relational graphs for cell nucleus segmentation in fluorescence microscopy images," IEEE Transactions on Medical Imaging, 32(6):1121-1131, 2013.
```
# References

