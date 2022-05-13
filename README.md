# dcm2png
A repository for comparing performance of open-source libraries for DICOM to PNG conversion


Performance: 
pydicom = 0.0749s
dcmj2pnm = 6.85777s
mogrify = 14.15s
convert2 = 13.86s

Using dask we can reduce the time by using all the cores to 9.5 seconds, but this works only for multiple images
and not for single

The mogrify utility needs some changes related to OpenCL and build the library again to make it run on GPU.
