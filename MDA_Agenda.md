# ANTs tutorial / workshop at MD Anderson

## Overview
  * Cooking show format
  * Using data described [here](http://www.nature.com/articles/sdata20153)
  * Supplemented with a couple of elderly subject datasets.

## Visualization
  * [ITK-snap](http://www.itksnap.org/pmwiki/pmwiki.php) for images
  * [Rstudio](https://www.rstudio.com) for statistics and plotting
  * [antsSurf](https://github.com/stnava/antsSurf) for surfaces
  * [antsVol](https://github.com/ntustison/antsVisualizationExamples) for rendering

## Datasets

  * A complete multi-modality subject http://files.figshare.com/1701182/PEDS012_20131101.zip
  * PTBP demographics [here](https://ndownloader.figshare.com/files/1699436)
  * PTBP tutorial data [here](https://www.dropbox.com/s/5p0vlx8en9uzbge/ ants_tutorial_data.zip?dl=1)
  * Elderly subject data [here (FIXME)](notyet)

-----------------------------------------------------------------

## Agenda

### August 11

Day 1: Registration, segmentation and framework

| Time             |     Activity                              | Presenter|
|:----------------:|-------------------------------------------|----------|
|  9:00 - 10:00    | Introduction, set-up, and ANTs overview   | NT |
| 10:00 - 10:30    | Coffee and questions/discussion           | -- |
| 10:30 - 11:15    | Going deeper into ANTs Registration       | NT |
| 11:15 - 12:00    | Introduction to ANTsR                     | BA |
| 12:00 -  1:00    | Lunch and questions/discussion            | -- |
|  1:00 -  2:00    | Templates and prior-based segmentation    | ?? |
|  2:00 -  2:30    | Coffee and questions/discussion           | -- |
|  2:30 -  3:30    | Segment new data with priors, RFs, etc    | NT |
|  3:00 -  4:00    | Research topics and/or discussion         | ?? |

### August 12

Day 2: Multivariate statistics, visualization and prediction

| Time             |     Activity                         |Presenter|
|:----------------:|--------------------------------------|----|
|  9:00 - 10:00    | Review of previous day               | NT |
| 10:00 - 10:30    | Coffee and questions/discussion      | -- |
| 10:30 - 11:30    | Let's perform a "real study"         | BA |
| 11:30 - 12:00    | Research topics and/or discussion    | ?? |
| 12:00 -  1:00    | Lunch and questions/discussion       | -- |
|  1:00 -  2:00    | Resting state fMRI in ANTsR          | BA |
|  2:00 -  2:30    | Coffee and questions/discussion      | ?? |
|  2:30 -  3:00    | Population statistics & visualization| ?? |
|  3:00 -  4:00    | Individual/group discussion          | ?? |


### August 11:  Registration, segmentation and framework

__Topics__

    * ANTs history & philosophy
        * ANTs origins in SyN
        * collaborators
        * open source and reproducibility
        * competition history
    * Development and interface with the user community
        * ITK
        * Github
        * sourceforge and github help forum
        * documentation
    * ANTs command line
    * Dependencies
        * CMake
        * ITK
        * VTK
    * Core programs
        * antsRegistration
        * Atropos
        * N4/N3*
        * KK
        * ImageMath
        * antsSurf/antsVol
        * antsAI
    * Core scripts
        * antsRegistrationSyN(Quick).sh
        * antsBrainExtraction.sh
        * antsAtroposN4.sh
        * antsCorticalThickness.sh
        * buildtemplateparallel.sh/antsMultivariateTemplateConstruction.sh
        * antsJointLabelFusion.sh
    * Data
        * Nature paper
        * figshare
        * data modifications for tutorial
    * ANTsR overview
    * template building
    * mapping other modalities
    * template building
    * mapping other modalities through the T1

__Questions to be addressed__

    * What is the history of ANTs/ANTsR?
    * Where can I download ANTs/ANTsR?
    * How do I install ANTs/ANTsR on my machine?
    * Who are the ANTs/ANTsR developers and contributors?
    * Where can I get help for problems with ANTs/ANTsR?
    * Can I contribute to ANTs/ANTsR?
    * How is ITK related to ANTs?
    * Where can I find ANTs documentation?
    * What is ANTSPATH?
    * What does ANTs not do?  (Motivate the use of ANTsR)


__Possible interactive activities__


    * Explore ANTs directory structure
    * Explore ANTs sourceforge/Github forum
    * Look at ITK doxygen
    * Update the ANTs and ANTsR repository
    * Set up ANTSPATH
    * Run r16/r85 registration
    * Create a T1-weighted template
    * Create a multivariate template
    * Create a symmetric template
    * Create priors for the template
    * Create cortical labels for the template
    * Apply priors to new data


### August 12: Multivariate statistics, visualization and prediction

__Topics__

* We will first refresh topics from day one and cover material that we missed.

* We will also refine day 2 material given the feedback from day 1.

* Statistical analyses with ANTs and ANTsR

__Questions to be addressed__

* How do I compute population statistics with ANTs data?

* How do I visualize statistical results?

* How do I perform predictive studies?  E.g. compute brainAge?

__Possible interactive activities__

* See: [ANTsTutorial](https://github.com/stnava/ANTsTutorial) for an overview of material.

    * ANTsR VBM

    * ANTsR brainAge

    * ANTsR dimensionality reduction

* See the examples [here](https://github.com/stnava/ANTsTutorial/blob/master/handout/antsGithubExamples.Rmd).
