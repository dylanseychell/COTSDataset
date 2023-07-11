# COTS (Common Objects of a Traveling Scientist) Dataset

<p align="right" style="text-align: right;">
  <strong>"a travel-themed dataset containing 120 different instances organized in a selection of scenes"</strong>
</p>
<br>
<p align="left" style="text-align: left;">
  <strong>"a multipurpose RGB-D dataset that enables the evaluation of a pipelined solution"</strong>
</p>

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
- [**Part 1 - Single Objects**](./Part%201%20-%20Single%20Objects/) - This directory contains single objects shot with a green background.
- [**Part 2 - Multiple Objects**](./Part%202%20-%20Multiple%20Objects/) - This directory contains different instances of specific scenes with multiple objects shot with a green background.
- [**Part 3 - Complex Background**](./Part%203%20-%20Complex%20Background/) - This directory contains different instances of specific scenes with multiple objects shot with a complex background.

## Documented Setup
To develop this dataset, a dedicated controlled environment was used. The setup is presented visually as a plan elevation below:
<p align="center">
  <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/b3804421-3d5c-434b-9534-ca0ea61b454d" style="display: block; margin: 0 auto; width: 100%; height: auto;">
</p><br>

The recordings took place in an indoor environment without any external natural lighting. The only source of light used was that of two auxiliary LED lighting with
modifiers that were targeted at the objects. Important considerations were made to ensure that the auxiliary lighting being used in the scene were not generating infra-red noise that would possibly affect negatively the quality of the captured depth map. In addition, a designated region on the surface was marked so that every object is placed within this region as this mark falls precisely within the camera’s field of view. Moreover, the configuration of the scene was measured and recorded, keeping the setup constant throughout the scene capturing process.

## Depth Maps
![seych5-3055647-large](https://github.com/mbar0075/COTSDataset/assets/103250564/e9ba9063-6b9a-4359-b8ae-92760e06149a)


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

