# HDRSR
This paper presents an algorithm for high dynamic range (HDR) and super-resolution (SR) imaging from a single image.

## Title of this work
high dynamic range and super resolution imaging system

## Abstract
This paper presents an algorithm for high dynamic range (HDR) and super-resolution (SR) imaging from a single image. First, we propose a new single image high dynamic range imaging (HDRI) method based on the Retinex approach and exploit a recent single image super-resolution (SR) method based on a convolutional neural network (CNN). Among many possible configurations of HDR and SR, we find an optimal system configuration and color manipulation strategy from the extensive experiments. Specifically, the best results are obtained when we first process the luminance component (Y) of input with our single image HDRI algorithm and then feed the enhanced HDR luminance to the CNN-based SR architecture that is trained by only luminance component. The ranges of chromatic components (U and V ) are just scaled in proportion to the enhanced HDR luminance, and then they are bicubic-interpolated or fed to the above CNN-based SR. Subjective and objective assessment for various experiments are presented to validate the effectiveness of the proposed HDR/SR imaging scheme.

