# BuildingFootprints
This project hopes to replicate Microsoft's building footprints project at https://github.com/Microsoft/USBuildingFootprints , which used ResNet34 and RefineNet (https://arxiv.org/pdf/1611.06612.pdf) for per-pixel classification. 

The source .tiff files from which the sample images are derived are in /N/dc2/projects/levee_ml/2016Hamilton. mosaic2.tif is a satellite image of Hamilton County, while bina1.tif is a grayscale image corresponding to the satellite image indicating where buildings are and aren't. Corresponding pairs of image slices (256x256 .tif files) are in /N/dc2/projects/levee_ml/hamiltondemo/citysample1 , split into train and test, and into (satellite) images and labels. training_images/0109_0040.tif corresponds to training_labels/0109_0040.tif , and so on. The satellite images are 3-channel RGB images, while the label images are 1-channel grayscale with 255 denoting building, 0 denoting non-building.