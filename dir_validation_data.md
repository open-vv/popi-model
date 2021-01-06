# Validation Data for Deformable Image Registration

## Motivation

We believe research on deformable image registration (DIR) of the lungs will greatly benefit from making image and validation data publicly available. Several 4D CT data sets, acquired at the Léon Bérard Cancer Center, can be downloaded here for use in your research. Along with the images, we provide large sets of manually identified landmarks, allowing you to validate your motion estimation.

We welcome all suggestions that can make this data more useful for you.  _David Sarrut_,  **[david.sarrut[at]creatis.insa-lyon.fr](mailto:david.sarrut@creatis.insa-lyon.fr)**


## Downloads

By downloading this data, you agreeing to follow these guidelines. When using any of the data provided for publications, please make reference to:

-   The institution from which they were obtained:  _the Léon Bérard Cancer Center & CREATIS lab, Lyon, France._
    
-   The article containing the description of this data:
    
    **J. Vandemeulebroucke, S. Rit, J. Kybic, P. Clarysse, and D. Sarrut.**  _**Spatiotemporal motion estimation for respiratory-correlated imaging of the lungs.**_  **In  _Med Phys_, 2011, 38(1), 166-178.**  [pdf](https://github.com/open-vv/popi-model/blob/master/Vandemeulebroucke2011.pdf "pdf")
    

The inhale-exhale image pairs were also used in

-   **J. Vandemeulebroucke, O. Bernard, S. Rit, J. Kybic, P. Clarysse, and D. Sarrut.**  _**Automated segmentation of a motion mask to preserve sliding motion in deformable registration of thoracic CT.**_  **In  _Med Phys_, 2012, 39(2), 1006-1015.**  [pdf](https://github.com/open-vv/popi-model/blob/master/Vandemeulebroucke2012.pdf "pdf")
    

The landmarks were identified using a software tool proposed by Keelin Murphy

-   **K. Murphy, B. van Ginneken, S. Klein, M. Staring, B. de Hoop, M. Viergever & J. Pluim.**  _**Semi-automatic construction of reference standards for evaluation of image registration.**_  **In  _Med Im Anal_, 2011, 15, 71-84.**
    

| Patient | Dicom Files | Reference Points | Reference Phase | MHD Files | Translation (Add this value to coordinates y for points to display them on the dicom, in mm) |
| ------- | -------------- | ------ | ------ | ------ | ------ |
| 1       | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/bl/dcm) | [Points](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/bl/pts) | 60 | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/bl/mhd) | 85.9375 |
| 2       | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/ng/dcm) | [Points](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/ng/pts) | 50 | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/ng/mhd) | 54.6875 |
| 3       | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/dx/dcm) | [Points](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/dx/pts) | 50 | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/dx/mhd) | 54.4921875 |
| 4       | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/gt/dcm) | [Points](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/gt/pts) | 50 | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/gt/mhd) | 55.46875 |
| 5       | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/mm2/dcm) | [Points](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/mm2/pts) | 50 | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/mm2/mhd) | 55.078125 |
| 6       | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/bh/dcm) | [Points](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/bh/pts) | 50 | [Images](http://www.creatis.insa-lyon.fr/~srit/POPI/MedPhys11/bh/mhd) | 55.078125 |


## Data Description

Images were acquired on a 16 Slice Brilliance CT Big Bore Oncology™ configuration (Philips). Breathing correlated information was obtained using the associated Pneumo Chest bellows™ (Lafayette Instruments). Each data set consists of ten 3D CT frames, respresenting a breathing cycle.

The landmarks were identified using a software tool proposed by Keelin Murphy (for a full description of the identification procedure followed, see  [[Vandemeulebroucke2012.pdf](https://github.com/open-vv/popi-model/blob/master/Vandemeulebroucke2012.pdf "[Vandemeulebroucke2012.pdf")]). For the first three patients, approximately a hundred landmarks were identified in all frames. For the remaining three patients, a hundred landmarks were provided in the inhale and exhale frame.

 Landmarks are defined in the MHD coordinate system. The coordinates in the Dicom Images are given in the CT scanner coordinate system while MHD images use the coordinate system of our Treatment Planing System that puts the origin at the center of the image in the Y direction compensating for the hight of the CT couch. To display landmarks in the Dicom Images, a Y translation must be applied, either to the Dicom Images or to the landmarks themselves, so that the origin is centered in the middle of the CT image in the Y direction.

## Other Useful Links

-   VV, a 4D image viewer can be downloaded from  [https://github.com/open-vv/vv](https://github.com/open-vv/vv)
    
-   More inhale-exhale image pairs of the thorax, along with landmarks, can be found on  [http://www.dir-lab.com/](http://www.dir-lab.com/)
    
-   More data sets for validation and evaluation in medical image processing can be found on  [http://www.vmip.org/](http://www.vmip.org/).


