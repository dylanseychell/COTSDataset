# COTS (Common Objects of a Traveling Scientist) Dataset

## Abstract
*Many modern computer vision systems include several modules that perform different
processing operations packaged as a single pipeline architecture. This generally introduces a challenge in
the evaluation process since most datasets provide evaluation data for just one of the operations. In this
paper, we present an RGB-D dataset that was designed from first principles to cater for applications that
involve salient object detection, segmentation, inpainting and blending techniques. This addresses a gap in
the evaluation of image inpainting and blending applications that generally rely on subjective evaluation due
to the lack of availability of comparative data. A set of experiments were carried out to demonstrate how the
COTS dataset can be used to evaluate these different applications. This dataset includes a variety of scenes,
where each scene is captured multiple times, each time adding a new object to the previous scene. This
allows for a comparative analysis at pixel level in image inpainting and blending applications. Moreover, all
objects were manually labeled in order to offer the possibility of salient object detection even in scenes that
contain multiple objects. An online test with 1267 participants was also carried out, and this dataset also
includes the click coordinates of users’ selection for every image, introducing a user interaction dimension
in the same RGB-D dataset. This dataset was also validated using state of the art techniques, obtaining an
F<sub>β</sub> of 0.957 in salient object detection and a mean (Intersection over Union) IoU of 0.942 in Segmentation.
Results demonstrate that the COTS dataset introduces novel possibilities for the evaluation of computer
vision applications.*

## Repository Structure

## Citation
To cite this paper, kindly use the following citation:

```bib
@ARTICLE{9340352,
  author={Seychell, Dylan and Debono, Carl James and Bugeja, Mark and Borg, Jeremy and Sacco, Matthew},
  journal={IEEE Access}, 
  title={COTS: A Multipurpose RGB-D Dataset for Saliency and Image Manipulation Applications}, 
  year={2021},
  volume={9},
  number={},
  pages={21481-21497},
  doi={10.1109/ACCESS.2021.3055647}}

```

The paper associated with the COTS dataset is available on IEEE: https://ieeexplore.ieee.org/document/9340352

<!--
A Multipurpose RGB-D Dataset for Inpainting and Saliency Applications

Paper associated with COTS can be found 

https://ieeexplore.ieee.org/document/9340352

To reference the COTS Dataset in your work please use the following citation

D. Seychell, C. J. Debono, M. Bugeja, J. Borg and M. Sacco, "COTS: A Multipurpose RGB-D Dataset for Saliency and Image Manipulation Applications," in IEEE Access, vol. 9, pp. 21481-21497, 2021, doi: 10.1109/ACCESS.2021.3055647.
-->
