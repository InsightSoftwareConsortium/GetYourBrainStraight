Back to the [Tutorials List](../../README.md#tutorials-list)

# Metadata Preservation for Brain Registration

## Instructors

- Matt McCormick (Kitware)
- Lydia Ng (Allen Institute for Brain Science)
- Dženan Zukić (Kitware)

## Tutorial Description

In this tutorial, we will explain why metadata preservation is important for brain image analysis,
explicitly identify the metadata required for registration, how the metadata can be preserved, and
how these techniques apply to the fMOST dataset studied in the hackathon.

Duration: 1.0 hours.

## Learning Outcomes

1. Understand why neuroimage registration metadata preservation is important for reproducible, scalable, and sustainable analysis. 
2. Identify the spatial image and transformation metadata required for provenance and future analysis.
3. Identify standard formats and software tools to store and work with this metadata.
4. Understand how this information was applied to the fMOST example dataset to address volumes stored in non-standard formats, with different brain orientations, and collected at varying resolutions.

## Approach and Materials

- [Presentation on the theory and practice of neuroimage metadata preservation](https://docs.google.com/presentation/d/e/2PACX-1vQy692yDVT7QljqfV4lfLjbUcIQZ1ePUSczk2YCCb-I1Fj0yIYypHV2ZT0Q58G_7RofZUOSDY6pOiqZ/pub?start=false&loop=false&delayms=3000)
- [ITK image grid: image's spatial metadata](https://mybinder.org/v2/gh/InsightSoftwareConsortium/GetYourBrainStraight/main?filepath=HCK01_2022_Virtual/Tutorials/MetadataPreservation/ITK_image_grid.ipynb)
- [OrientImageFilter for consistent anatomical orientation](https://mybinder.org/v2/gh/InsightSoftwareConsortium/GetYourBrainStraight/main?filepath=HCK01_2022_Virtual/Tutorials/MetadataPreservation/Orient_filter.ipynb)
- [ITK-NiBabel spatial metadata to 4x4 affine matrix and back](https://mybinder.org/v2/gh/InsightSoftwareConsortium/GetYourBrainStraight/main?filepath=HCK01_2022_Virtual/Tutorials/MetadataPreservation/LPS-RAS-4x4.ipynb)
- [C++ example](./AccessSpatialMetadata/Code.cxx) with corresponding [Python example](./AccessSpatialMetadata/Code.py).

## Background and References

- The [ITK Software Guide](https://itk.org/ItkSoftwareGuide.pdf)

## Run the Tutorial

There are a few ways to run these tutorials.

### On the Web, with Binder

Just click on the links above, and wait a few minutes until a Jupyter server starts.

### Locally, with Python from Python.org or a System Python

First, install [Python](https://www.python.org/downloads/release/python-3912/),
if not already available.

Next, install the required dependencies::
```bash
   python -m pip install jupyter matplotlib numpy
   python -m pip install --upgrade --pre itk
```
Then, clone the repository::
```bash
  git clone https://github.com/InsightSoftwareConsortium/GetYourBrainStraight.git
  cd GetYourBrainStraight/HCK01_2022_Virtual/Tutorials/MetadataPreservation
```
And start Jupyter::
```bash
  python -m jupyter notebook
```
