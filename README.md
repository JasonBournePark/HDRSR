* More contents will be disclosed after finishing review process.

# HDRSR
This paper presents an algorithm for high dynamic range (HDR) and super-resolution (SR) imaging from a single image.
<br><br>
## Title of this Work
high dynamic range and super resolution imaging system
<br><br>
## Abstract
This paper presents an algorithm for high dynamic range (HDR) and super-resolution (SR) imaging from a single image. First, we propose a new single image high dynamic range imaging (HDRI) method based on the Retinex approach and exploit a recent single image super-resolution (SR) method based on a convolutional neural network (CNN). Among many possible configurations of HDR and SR, we find an optimal system configuration and color manipulation strategy from the extensive experiments. Specifically, the best results are obtained when we first process the luminance component (Y) of input with our single image HDRI algorithm and then feed the enhanced HDR luminance to the CNN-based SR architecture that is trained by only luminance component. The ranges of chromatic components (U and V ) are just scaled in proportion to the enhanced HDR luminance, and then they are bicubic-interpolated or fed to the above CNN-based SR. Subjective and objective assessment for various experiments are presented to validate the effectiveness of the proposed HDR/SR imaging scheme.
<br><br>
## Related Work
### CNN-based Single Image Super Reolution
#### [SRCNN] Image Super-Resolution Using Deep Convolutional Networks <paper-button> <a href="http://mmlab.ie.cuhk.edu.hk/projects/SRCNN.html">Link</a> </paper-button>
#### [VDSR] Accurate Image Super-Resolution Using Very Deep Convolutional Networks <paper-button> <a href="https://arxiv.org/abs/1511.04587">Link</a> </paper-button>
### Image Enhancement and HDR Imaging
#### [FbEM] A fusion-based enhancing method for weakly illuminated images <paper-button> <a href="http://www.sciencedirect.com/science/article/pii/S0165168416300949">Link</a> </paper-button>
#### [NPEA] Naturalness Preserved Enhancement Algorithm for Non-Uniform Illumination Images <paper-button> <a href="http://ieeexplore.ieee.org/document/6512558/">Link</a> </paper-button>
#### [LIME] Low-Light Image Enhancement via Illumination Map Estimation <paper-button> <a href="http://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7782813">Link</a> </paper-button>
<br><br>
## Implementation
#### HDR Imaging (To be uploaded)
#### CNN-based Super Resolution Imaging (To be uploaded)
<br><br>
## Experimental Results
#### □ Proposed HDRI results
<p align="center"><img src="/Figures/Proposed_HDRI.png" width="700"></p>
An example of our HDRI process; (top left) input LDR, (top right) output HDR image; (the second row) generated virtual illuminations I_k; (the third row) reproduced Y_k; (the last row) weight maps w_k. 
<br><br>

<p align="center">
<img src="/Figures/Fig_HDRI_Comparison.png" width="700"> 
</p>
Visual comparison of enhanced images from the MMPSG LDR images. (From left to right) input LDR images, enhanced images by FbEM, LIME, NPEA and the proposed algorithm.
<br>

#### □ Super-resolved results by VDSR
<p align="center">
<img src="/Figures/Proposed_VDSR.png" width="700"> 
</p>
HR images by interpolation and VDSR; (from left to right) interpolated HR image, input HR image and super-resolved HR image by VDSR.
<br>

#### □ HDR-SR test results
Visual comparison for an image of natural scene, (a) reference LDR/HR image, (b) interpolated LDR/HR image, (c) super-resolved LDR/HR image, (d-e) HDR/HR images generated by SR(YpUV)-HDR and SR(RGB)-HDR strategies, (f-g) HDR/HR images generated by HDR-SR(YpUV) and HDR-SR(RGB) strategies, (h-n) magnified images of the indicated areas in each image of (a-g).

<p align="center">
<img src="/Figures/small_Exp_VisualComp_C11.png" width="500"> 
</p>
*this is small-size sample image, please download the original image to compare the results.
<br>

<p align="center">
<img src="/Figures/small_Exp_VisualComp_C27.png" width="500"> 
</p>
*this is small-size sample image, please download the original image to compare the results.
<br>

<p align="center">
<img src="/Figures/small_Exp_VisualComp_C33.png" width="500"> 
</p>
*this is small-size sample image, please download the original image to compare the results.
<br>

<p align="center">
<img src="/Figures/small_Fig_Exp_VisualComp_C35.png" width="500"> 
</p>
*this is small-size sample image, please download the original image to compare the results.
<br>
