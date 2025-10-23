---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

## Project 1. 3D reconstruction for endoscopy, dermatology 
The 3D reconstruction is the process of recovering the shape or structure of the
surfaces that are seen in images. This research topic, which has occupied researchers
for decades, is still topical, particularly because of the numerous application fields
of 3D scene construction: computer aided geometric design (CAGD), computer
graphics, computer animation, computer vision, medical imaging, computational
science, virtual reality, digital media, etc. The goal of this project is to propose a 3D mosaicing algorithm for endoscopic scenes
under the assumption that the observed surfaces are (almost) rigid. We want to construct
extended fiew-of-views (FoVs) in a robust and accurate way.

Among many techniques for 3D reconstruction, we used the Structure from Motion technique (SfM)
which aims to recover 3D structures of a stationary (non-deformable) surface using
a set of 2D images. SfM methods require the knowledge of numerous and accurate
point correspondences between images. The correspondence of homologous points is
usually given in the form of point-tracks which are used to simultaneously estimate
the camera trajectory and a 3D point cloud located on the surface to be recovered.
SfM is a widely employed technique that is able to reconstruct a great variety of
scenes using only images acquired from different viewpoints. However, applying this technique to endoscopic images in general is difficult, and in gastroscopic images it is a big challenge.
This is mainly due to the challenging lighting conditions, specular reflections, and low-texture characteristics of endoscopic images.
To make the SfM technique applicable to endoscopic data, we proposed to integrate an Optical Flow method into the SfM framework, which effectively addresses the problem of textureless image regions.

A complete pipeline for 3D reconstruction in our project includes the steps: Pre-processing -> **SfM** -> Multi-view stereo -> Meshed surface computation and refinement -> Multiple view mesh texturing.
Several scientific papers were published in this project, you can find them in the links below.
- **Tan-Binh Phan**, Dinh-Hoan Trinh, Dominique Lamarque, Didier Wolf, Christian Daul. 
  *3D surface reconstruction using dense optical flow combined to feature matching: Application to endoscopy.*  
  GRETSI (2019). [[Link]](https://hal.science/hal-02271615/)

- **Tan-Binh Phan**, Dinh-Hoan Trinh, Dominique Lamarque, Didier Wolf, Christian Daul.  
  *Dense optical flow for the reconstruction of weakly textured and structured surfaces: Application to endoscopy.*  
  IEEE ICIP (2019). [[Link]](https://ieeexplore.ieee.org/abstract/document/8802948)

- **Tan Binh Phan**, Dinh Hoan Trinh, Didier Wolf, Christian Daul. 
  *Optical flow-based structure-from-motion for the reconstruction of epithelial surfaces.*  
  Pattern Recognition (2020). [[Link]](https://www.sciencedirect.com/science/article/abs/pii/S0031320320301941)

- Rafael Bayareh Mancilla, **Tan-Binh Phan**, et al.  
  *Anatomical 3D modeling using IR sensors and radiometric processing based on structure from motion: Towards a tool for the diabetic foot diagnosis.*  
  Sensors (2021). [[Link]](https://www.mdpi.com/1424-8220/21/11/3918)
**Application**: From the medical point of view, the proposed SfM methods can reconstruct surfaces acquired for various endoscopic scenes and imaging modalities. The extended
FOV images facilitate the detection of abnormal regions (e.g., with polyps) or inflammations (e.g., inflammations around the pyloric antrum region of the stomach).
Besides that, the surfaces of the same region reconstructed by the proposed SfM algorithms for two or more examinations help to diagnose a lesion evolution or to assess
the remission of a tissue after surgery for instance. For the tested medical applications, the proposed 3D reconstruction pipeline led systematically to consistent
3D shapes (in accordance with the anatomy of the organ), without discontinuities of textures or structures, as well as with an acceptable resolution regardless of the
location observed on the surface. Textured 3D images of the internal organ wall surfaces also support the exchange of information between physicians of different
specialties.  

## Project 2. Non-Rigid Structure from Motion for the esophagus
...

## Project 3. 3D echocardiography
This work proposed a 3D pipeline for motion estimation of myocardial which consists of four sequential chains. Starting with the pre-processing step, the Raw-Dicom/Dicom (Digital imaging and communications in medicine) les are processed to the correct format files which are used as the input of the second step, that is the segmentation of myocardial.
The endocardium and epicardium delineated in the segmentation are used for the tracking process which computed the movement of the myocardium in each frame. The aim of the final step is to estimate the velocity fields and give a framework to evaluate the motion of the myocardium.

## Project 4. Tomography reconstruction
- Ombeline de La Rochefoucauld,...,**Tan-Binh Phan**, et al.  
  *Element differentiation with a Hartmann based X-ray phase imaging system.*  
  Nondestructive Testing and Evaluation (2022). [[Link]](https://doi.org/10.1080/10589759.2022.2095383)
