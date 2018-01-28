# DataScienceBowl2018

## Spot Nuclei. Speed Cures.
Imagine speeding up research for almost every disease, from lung cancer and heart disease to rare disorders. The 2018 Data Science Bowl offers our most ambitious mission yet: create an algorithm to automate nucleus detection.

We’ve all seen people suffer from diseases like cancer, heart disease, chronic obstructive pulmonary disease, Alzheimer’s, and diabetes. Many have seen their loved ones pass away. Think how many lives would be transformed if cures came faster.

By automating nucleus detection, you could help unlock cures faster—from rare disorders to the common cold. Want a snapshot about the 2018 Data Science Bowl? [View this video.](https://www.youtube.com/watch?v=eHwkfhmJexs&feature=youtu.be).

## Why nuclei?
Identifying the cells’ nuclei is the starting point for most analyses because most of the human body’s 30 trillion cells contain a nucleus full of DNA, the genetic code that programs each cell. Identifying nuclei allows researchers to identify each individual cell in a sample, and by measuring how cells react to various treatments, the researcher can understand the underlying biological processes at work[Check out this video overview to find out more.](https://datasciencebowl.com/2018dsbtutorial/)

By participating, teams will work to automate the process of identifying nuclei, which will allow for more efficient drug testing, shortening the 10 years it takes for each new drug to come to market.

## What will participants do?
Teams will create a computer model that can identify a range of nuclei across varied conditions. By observing patterns, asking questions, and building a model, participants will have a chance to push state-of-the-art technology farther.

Visit [DataScienceBowl.com](www.datasciencebowl.com) to:
* Sign up to [receive news](https://datasciencebowl.com/contact/) about the competition
* Learn about the [history of the Data Science Bowl](https://datasciencebowl.com/competitions/) and past competitions
* Read our [latest insights](https://datasciencebowl.com/data-science-insights/) on emerging analytics techniques

![](https://storage.googleapis.com/kaggle-media/competitions/dsb-2018/dsb.jpg)

## Data 
This dataset contains a large number of segmented nuclei images. The images were acquired under a variety of conditions and vary in the cell type, magnification, and imaging modality (brightfield vs. fluorescence). The dataset is designed to challenge an algorithm's ability to generalize across these variations.

Each image is represented by an associated ImageId. Files belonging to an image are contained in a folder with this ImageId. Within this folder are two subfolders:

* images contains the image file.
* masks contains the segmented masks of each nucleus. This folder is only included in the training set. Each mask contains one nucleus. Masks are not allowed to overlap (no pixel belongs to two masks).

The second stage dataset will contain images from unseen experimental conditions. To deter hand labeling, it will also contain images that are ignored in scoring. The metric used to score this competition requires that your submissions are in run-length encoded format. Please see the evaluation page for details.

As with any human-annotated dataset, you may find various forms of errors in the data. You may manually correct errors you find in the training set. The dataset will not be updated/re-released unless it is determined that there are a large number of systematic errors. The masks of the stage 1 test set will be released with the release of the stage 2 test set.
[Stage 1 Sample Submission](https://www.kaggle.com/c/data-science-bowl-2018/download/stage1_sample_submission.csv.zip)
[Stage 1 Test](https://www.kaggle.com/c/data-science-bowl-2018/download/stage1_test.zip)
[Stage 1 Train](https://www.kaggle.com/c/data-science-bowl-2018/download/stage1_train.zip)
[Stage 1 Train Label](https://www.kaggle.com/c/data-science-bowl-2018/download/stage1_train_labels.csv.zip)

### File descriptions

+ /stage1_train/* - training set images (images and annotated masks)
+ /stage1_test/* - stage 1 test set images (images only, you are predicting the masks)
+ /stage2_test/* (released later) - stage 2 test set images (images only, you are predicting the masks)
+ stage1_sample_submission.csv - a submission file containing the ImageIds for which you must predict during stage 1
+ stage2_sample_submission.csv (released later) - a submission file containing the ImageIds for which you must predict during stage 2
+ stage1_train_labels.csv - a file showing the run-length encoded representation of the training images. This is provided as a convenience and is redundant with the mask image files.
