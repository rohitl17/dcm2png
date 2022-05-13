# dcm2png
A repository for comparing performance of open-source libraries for DICOM to PNG conversion


Performance: 
1) pydicom = 0.0749s
2) dcmj2pnm = 6.85777s
3) mogrify = 14.15s
4) convert2 = 13.86s

Using dask we can reduce the time by using all the cores to 9.5 seconds, but this works only for multiple images and not for single image.

The mogrify utility needs some changes related to OpenCL and build the library again to make it run on GPU.
