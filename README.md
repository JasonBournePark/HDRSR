# HDRSR
This paper presents an algorithm for high dynamic range (HDR) and super-resolution (SR) imaging from a single image.
<br><br>
## Title of this Work
high dynamic range and super resolution imaging system
<br><br>
## Abstract
This paper presents an algorithm for high dynamic range (HDR) and super-resolution (SR) imaging from a single image. First, we propose a new single image high dynamic range imaging (HDRI) method based on the Retinex approach and exploit a recent single image super-resolution (SR) method based on a convolutional neural network (CNN). Among many possible configurations of HDR and SR, we find an optimal system configuration and color manipulation strategy from the extensive experiments. Specifically, the best results are obtained when we first process the luminance component (Y) of input with our single image HDRI algorithm and then feed the enhanced HDR luminance to the CNN-based SR architecture that is trained by only luminance component. The ranges of chromatic components (U and V ) are just scaled in proportion to the enhanced HDR luminance, and then they are bicubic-interpolated or fed to the above CNN-based SR. Subjective and objective assessment for various experiments are presented to validate the effectiveness of the proposed HDR/SR imaging scheme.
<br><br>
<br><br>
## Related Work
##### [SRCNN] Accurate image super-resolution using very deep convolutional networks <paper-button> <a href="http://mmlab.ie.cuhk.edu.hk/projects/SRCNN.html">Link</a> </paper-button>
##### [VDSR] LIME: Low-Light Image Enhancement via Illumination Map Estimation <paper-button> <a href="https://arxiv.org/abs/1511.04587">Link</a> </paper-button>
##### [FbEM] A fusion-based enhancing method for weakly illuminated images <paper-button> <a href="http://www.sciencedirect.com/science/article/pii/S0165168416300949">Link</a> </paper-button>
<br><br>
<br><br>
## Experimental Results
#### Result #1 for test images of backlighting conditions
<p align="center">
<img src="/Paper_Images/Figure_Exp_Rst_BL1.png" width="700"> 
<img src="/Paper_Images/Figure_Exp_Rst_BL2.png" width="700"> 
</p>

##### [Results for the image.From top left to bottom right: input image, result of CLAHE, CVC, MSR, FbEM,	LIME, NPEA and proposed method.]

#### Result #2 for test images of low light conditions
<p align="center">
<img src="/Paper_Images/Figure_Exp_Rst_Low1.png" width="700"> 
<img src="/Paper_Images/Figure_Exp_Rst_Low2.png" width="700"> 
</p>

##### [Results for the image. From top left to bottom right: input image, result of CLAHE, CVC, MSR, FbEM,	LIME, NPEA and proposed method.]

#### Result #3 for a test image of low light conditions
<p align="center">
<img src="/Paper_Images/Figure_Exp_Rst_NonUni.png" width="700"> 
</p>
