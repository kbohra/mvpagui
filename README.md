# mvpagui
MVPA GUI ( weblink: https://sites.google.com/site/mvpagui/home)

# About MVPAGUI Software
**************************************
Functional magnetic resonance imaging (fMRI) is a medical imaging method which indirectly measures brain activity by measuring changes in blood-oxygenation levels from 3D snapshots of the brain every few seconds. Exposing a subject to different kind of stimuli or tasks systematically during the fMRI scan causes different parts of the brain to activate. FMRI signal can be analyzed to find out the characteristics of these activations and any systematic activation differences under different stimuli/tasks. Multivariate pattern recognition and classification algorithms, as known as multivoxel pattern analyses (MVPA) methods in the neuroimaging community, have been recently applied to fMRI data to classify between different brain “states” or “conditions” resulting from different stimuli/tasks. MVPA methods have been gaining popularity in neuroimaging and there is need for user-friendly graphical user interface (GUI) software which implements these methods

Project Video Demo 
Link: https://www.youtube.com/watch?v=bt9bDW-q7Yk

Project Documents link: https://sites.google.com/site/mvpagui/downloads

# Design Overview and Implementation
*************************************
In this project, we implemented a MATLAB-based graphical user interface (GUI) tool which can read 
4D-Nifti fMRI data from the brain, and does classification of different brain “states” or “conditions” using various supervised machine learning algorithms. The algorithms which are implemented in the toolbox include linear discriminant analysis, neural networks, logistic regression, sparse multinomial logistic regression, ridge regression, and support vector machines. The toolbox allows the user to mask the brain and focus on only the anatomical parts she/he is interested in. The tool accommodates choosing between various types of inputs which describe the fMRI experiment stimuli/tasks and it provides a detailed visualization of results. The GUI designed here gives the user the flexibility to easily modify different parameter values of interest of the selected classification algorithm being applied.
An important feature of this GUI design is that one can save and load all the input parameters such as the classification algorithm selected, its parameters, the input data used for classification, etc. for a particular analysis. The results of classification can also be saved and loaded. This saves time for the user to easily go through particular analysis and its results in future if needed. We use some of the open-source SPM functions.

![alt text](https://github.com/kbohra/mvpagui/blob/master/images/mvpagui_image.png)


                                                   ABSTRACT
A SOFTWARE FOR MULTIVOXEL PATTERN ANALYSIS OF FUNCTIONAL MAGNETIC RESONANCE IMAGING DATA

Kushal Bohra, MS

Texas A&M University

Advisor: Unal Sakoglu, PhD

Functional magnetic resonance imaging (fMRI) is a medical imaging modality
which enables taking 3D snapshots of the whole brain usually every few seconds with approximately 3-30 millimeter-cube resolution. FMRI signal is a blood-oxygenation-level-dependent (BOLD) signal, which is an indirect measure of the brain’s neural activity. This technique relies on the fact that cerebral blood flow and neuronal activation are coupled. Exposing the subject to different kind of stimuli or tasks systematically during an fMRI scan causes different parts of the brain to activate. FMRI signals can be analyzed to find out the characteristics of these activations and any systematic differences between the activations under different stimuli and tasks. Multivariate pattern recognition and classification algorithms, also known as multivoxel pattern analysis (MVPA) in the neuroimaging community, have been recently applied to fMRI data and it has been gaining popularity. MVPA of fMRI data have allowed classification of different brain states under different stimuli or task conditions. For example, it is possible to distinguish, based on the fMRI data alone, whether a subject was looking at faces vs. tools, tools vs. houses etc. with a good specificity and sensitivity. However, the MVPA functions or tools that have been developed specifically for fMRI are not user-friendly. Data analysis require significant coding/programming by researchers, who are mostly psychologists, neurologists or neuroscientists
In this work, we developed a user-friendly, MATLAB-based GUI toolbox that allows fast, efficient and intuitive analysis of fMRI data. Many pattern recognition/classification functions, which are written for general 2-dimensional data, already exist in MATLAB. These functions were expanded to include the latest pattern recognition/classification analysis algorithms such as support-vector machines with multi-class support. These and already existing functions were tailored to analyze the fMRI data, which are 4-dimensional (space-time) and stored in a different data format (NIfTI-1/.nii) other than MATLAB’s data format (.mat). We tested our toolbox by doing a complete analysis of the six-subject fMRI dataset by Haxby et al., 2001 “Faces and Subjects in Ventral Temporal Cortex” and compared classification results from different classification algorithms.


