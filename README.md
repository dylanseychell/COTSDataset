# COTS (Common Objects of a Traveling Scientist) Dataset

<p align="right" style="text-align: right;">
  <strong>"a travel-themed dataset containing 120 different instances organized in a selection of scenes"</strong>
</p>
<br>
<p align="left" style="text-align: left;">
  <strong>"a multipurpose RGB-D dataset that enables the evaluation of a pipelined solution"</strong>
</p>


https://github.com/mbar0075/COTSDataset/assets/103250564/b8be54dd-35f6-40c0-bdc6-8c419f08ac06


## Abstract
<p align="justify">
<i>Many modern computer vision systems include several modules that perform different
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
vision applications.
</i>
</p>

## Repository Structure
- [**Part 1 - Single Objects**](./Part%201%20-%20Single%20Objects/) - This directory contains single objects shot with a green background.
- [**Part 2 - Multiple Objects**](./Part%202%20-%20Multiple%20Objects/) - This directory contains different instances of specific scenes with multiple objects shot with a green background.
- [**Part 3 - Complex Background**](./Part%203%20-%20Complex%20Background/) - This directory contains different instances of specific scenes with multiple objects shot with a complex background.

## Documented Setup
To develop this dataset, a dedicated controlled environment was used. The setup is presented visually as a plan elevation below:
<p align="center">
  <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/b3804421-3d5c-434b-9534-ca0ea61b454d" style="display: block; margin: 0 auto; width: 100%; height: auto;">
</p><br>
<p align="justify">
The recordings took place in an indoor environment without any external natural lighting. The only source of light used was that of two auxiliary LED lighting with
modifiers that were targeted at the objects. Important considerations were made to ensure that the auxiliary lighting being used in the scene were not generating infra-red noise that would possibly affect negatively the quality of the captured depth map. In addition, a designated region on the surface was marked so that every object is placed within this region as this mark falls precisely within the camera’s field of view. Moreover, the configuration of the scene was measured and recorded, keeping the setup constant throughout the scene capturing process.
</p>

<p align="center">
  <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/99b2098c-408d-4270-aad5-d2ec2d01ea8d" style="display: block; margin: 0 auto; width: 70%; height: auto;">
</p><br>

## Depth Maps
<p align="center">
  <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/e9ba9063-6b9a-4359-b8ae-92760e06149a" style="display: block; margin: 0 auto; width: 70%; height: auto;">
</p><br>

## Online Test
<table style="border: none;">
  <tr style="border: none;">
    <td style="text-align: left; border: none;" width="50%">
      <p align="justify" style>
        The evaluation of saliency detection algorithms and frameworks is one of the main aims of this paper. For this aim to be reached, the color images and their corresponding depth maps and objects masks were required to be accompanied by data so that it can illustrate better how humans can relate to the dataset. This was achieved through the use of an online test that was designed to reach this objective. </br></br> The main aim behind this experiment was to present the users with a color image from the dataset and analyze which region within the image they believe is the most salient. </br></br> The multi-level <strong>Data-Flow diagram</strong> presented on the right displays the main architectural modules of the aforementioned process.
      </p>
    </td>
    <td style="text-align: right;">
      <p align="center">
      <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/7f0dcc10-d2a3-4cda-82b8-c937e9febbde" alt="Image" width="60%" style="display: block; margin: 0 auto;">
      </p>
    </td>
  </tr>
</table>

## Annotation Maps
<p align="justify">
The average annotation map of the MSRA10K dataset shows that the salient objects in this dataset are biased towards its center. This bias was also considered in the design of the COTS dataset and as demonstrated below, this was mitigated accordingly by spreading salient objects further within the scene.
</p>
<table style="border: none;">
  <tr style="border: none;">
    <td style="text-align: left; border: none;" width="50%">
      <p align="center">
        <strong>COTS Dataset</strong></br>
      <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/fb749c28-9278-4a0a-bbc0-4aba69631882" alt="Image" width="60%" style="display: block; margin: 0 auto;">
      </p>
    </td>
    <td style="text-align: right;">
      <p align="center">
        <strong>MSRA10K Dataset</strong></br>
      <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/8a168784-793e-46a4-a471-0e89850149a4" alt="Image" width="45%" height="70%" style="display: block; margin: 0 auto;">
      </p>
    </td>
  </tr>
</table>

## Dataset Usage
### Saliency
The COTS dataset is an excellent resource for evaluating saliency ranking techniques. An example of its use can be seen below:
<p align="center">
  <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/5f115083-c140-4303-9f1a-ade61dae4b9d" style="display: block; margin: 0 auto; width: 60%; height: auto;">
</p>

### Inpainting
The COTS dataset is ideal for comparing different inpainting techniques. The pipeline of usage of the aforementioned dataset can be seen below:
<p align="center">
  <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/6aff0d13-ff9f-41e7-ba81-a99e5d1f5e3f" style="display: block; margin: 0 auto; width: 40%; height: auto;">
</p>

The following paper demonstrates how the COTS dataset can be used to objectively evaluate inpainting algorithms and make results more comparable:
```bib
@INPROCEEDINGS{9140597,
  author={Seychell, Dylan and Debono, Carl J.},
  booktitle={2020 IEEE 20th Mediterranean Electrotechnical Conference ( MELECON)}, 
  title={An Approach for Objective Quality Assessment of Image Inpainting Results}, 
  year={2020},
  volume={},
  number={},
  pages={226-231},
  doi={10.1109/MELECON48756.2020.9140597}}

```
Additionally, this paper is also available on IEEE: https://ieeexplore-ieee-org.ejournals.um.edu.mt/document/9140597

### Blending
The COTS dataset can also be used to evaluate content blending or addition techniques in a similar manner to inpainting techniques. The pipeline of usage of the aforementioned dataset can be seen below:
<p align="center">
  <img src="https://github.com/mbar0075/COTSDataset/assets/103250564/4bb70e85-11e7-42f3-8f10-402f77d6bc58" style="display: block; margin: 0 auto; width: 40%; height: auto;">
</p>

## Future Work
<p align="justify">
This dataset also provides a number of opportunities in evaluating modern computer vision techniques and architectures. COTS is being made available for free for everyone to use as an open-source project. This current version of the COTS dataset is focused on a plain green background. This was originally intended to allow for chroma-key background replacement and therefore increase the variety and complexity of the data. Future iterations of this dataset can potentially include a set of scenes with more a more complex natural background that would increase the evaluation possibilities upon it.
</p>

## Acknowledgements
<p align="justify">
The authors would like to thank Mr. Ryan Azzopardi, the professional photographer who assisted the team in the setting up of the studio and with the provision of lighting equipment for this setup. They also thankful to all the anonymous 1267 participants of the online test who dedicated time to go through the process and provide such precious feedback and information.
</p>

## Accessing Dataset
To access this dataset, kindly use the following code:

```python
# Packages Install
!pip install gitpython
import git
import shutil
import os

# Cloning repository
repo_url = 'https://github.com/dylanseychell/COTSDataset.git'
repo_dir = 'COTSDataset'  # Directory to clone the repository into
git.Repo.clone_from(repo_url, repo_dir)

# Defining paths
part1_single_objects = os.path.join(repo_dir, "Part 1 - Single Objects")
part2_multiple_objects = os.path.join(repo_dir, "Part 2 - Multiple Objects")
part3_complex_background = os.path.join(repo_dir, "Part 3 - Complex Background")

print("Repository cloned successfully.")
```

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

