## Functional parcellation for the anterior temporal lobe: a large-scale meta-analysis

This repository contains code, data, and results for our preliminary meta-analysis for functional parcellation in the anterior temporal lobe.

The codes are based on previous work parcellating MFC and LFC (de la Vega et al., 2016; 2018) and later DMN network (Wang, Taren & Smith, 2017): 

https://github.com/adelavega/neurosynth-mfc

https://github.com/adelavega/neurosynth-lfc

https://github.com/DVS-Lab/dmn-parcellation

(or https://github.com/neurosynth/neurosynth)

As instructed by the above authors, the main results can be produced following Clustering, Coactivation and Functional preference profiles.


### Requirements

I ran the analyses under WSL. I first created a virtual environment and pip install all required packages. This is different from the original suggestions. The mix of pip and conda install caused a few problems for me. 

The requirement.txt included all the packages for a stable environment for me (not a smart way but it worked). I first pip install the txt file and then the other packages as suggested by de la Vega (2016, 2018), which are listed below:

Python 2.7.x

For analysis:
- Neurosynth
- Scipy/Numpy
- Scikit-learn
- joblib
- nibabel 1.x (this is very important for the codes to work!)

For visualization:
- Pandas
- nilearn
- seaborn
- matplotlib



### Unzip pre-generated Neurosynth dataset prior to analysis
For topic-based meta-analysis, one should add features with topic information (i.e., not raw feature txt file with all features)
I used 0.6 version of Neurosynth dataset (available in July 2015, with 11406 fMRI studies).
