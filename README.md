# In Situ Lymphatic Imaging System (ISLIS)
LabVIEW VIs used in the following two papers by _Kassis et al._:

1. [Dual-channel in-situ optical imaging system for quantifying lipid uptake and lymphatic pump function (2012)](http://biomedicaloptics.spiedigitallibrary.org/article.aspx?articleid=1352568 "Dual-channel in-situ optical imaging system for quantifying lipid uptake and lymphatic pump function (2012)")
2. [Postprandial lymphatic pump function after a high-fat meal: a characterization of contractility, flow, and viscosity (2016)](http://ajpgi.physiology.org/content/310/10/G776 "Postprandial lymphatic pump function after a high-fat meal: a characterization of contractility, flow, and viscosity (2016)")

The process is composed of three steps:

1. **Stabilizing**: _in vivo_ imaging produces very substantial motion artifacts. This is especially true around the small intestine.
2. **Rotating**: to make the vessel align with parallel to the horizontal, thus making lymphocyte velocity measurements easier.
3. **Measuring diameter changes**: the two vessel walls initially marked by the user are tracked over time.
4. **Measuring lymphocyte velocity**: this is accomplished by tracking cells moving within the vessel walls.

_Please note this code is not production ready. It was put together quickly for a research project, but it works well._

## Installation
These LabVIEW VIs were originally written in LabVIEW 2014. I have recently upgraded them to version 2017. You need the following installed in order to use them:

1. LabVIEW 2017 (or another compatible version)
2. NI Vision Development Module 2017 (or another compatible version)

Simply clone the repository to your own computer.

## Usage
The VIs assume that the videos are in AVI format and that all segments are contained within the same folder. Simply run the VI from the appropriate folder to carry out the processing task on all the videos in the folder. Usually you would stabilize > rotate > measure. Please cite one of the papers mentioned earlier with any academic or commercial use.

## Contributors
If you have any improvements in mind please feel free to contribute to the project via Github. Make sure you use LabVIEW 2017. If you encounter issues running any part of the VIs please raise the issue on Github and I'll try to address it.
