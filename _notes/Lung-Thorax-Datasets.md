---
title: Recent Datasets for Lung Diseases
toc: true
season: winter
tags: lung
---

Related Documents: [[NIH-chestX14-vs-stanford-chestxpert]]

## Lung Diseases - Datasets and Models

Chest radiology (commonly refereed as chect radiograph or ChextX) is one of the most common imaging modalities in the world. It usually is captures as two views - frontal and side. It is first kind of imaging and is used in several kind of thorax disorders.

Certain kind of disorders are extremely difficult to be diagnosed from ChestX. Either experts and/or additional imaging is often needed to make a disgnosis.
Given their common nature, there are three major open public datasets available for this:
+ [ChestXpert](https://stanfordmlgroup.github.io/competitions/chexpert/)
+ [ChestXray-NIHCC](https://nihcc.app.box.com/v/ChestXray-NIHCC)
+ [MIMIC-CXR](https://physionet.org/content/mimic-cxr/2.0.0/)


![Figure 1: Sample ChestX Images](lung-xray-sample.png)

All of these datasets have labels for following 14 thorax conditions.

### Stanford ChestXpert

+ contains 224,316 CXRs, from 65,240 patients
+ 70% of the images come from 31% of the subjects
+ labeling is automted based on basic NLP


#### Distribution of Thorax conditions in ChestXpert

|      Condition       |    Positive    |   Uncertain    |    Negative     |
|:--------------------:|:--------------:|:--------------:|:---------------:|
|      No Finding      | 16627 (8.86%)  |    0 (0.0%)    | 171014 (91.14%) |
|   Enlarged Cadiom.   |  9020 (4.81%)  | 10148 (5.41%)  | 168473 (89.78%) |
|   **Cardiomegaly**   | 23002 (12.26%) |  6597 (3.52%)  | 158042 (84.23%) |
|     Lung Lesion      |  6856 (3.65%)  |  1071 (0.57%)  | 179714 (95.78%) |
|     Lung Opacity     | 92669 (49.39%) |  4341 (2.31%)  |  90631 (48.3%)  |
|      **Edema**       | 48905 (26.06%) | 11571 (6.17%)  | 127165 (67.77%) |
|  **Consolidation**   | 12730 (6.78%)  | 23976 (12.78%) | 150935 (80.44%) |
|      Pneumonia       |  4576 (2.44%)  | 15658 (8.34%)  | 167407 (89.22%) |
|   **Atelectasis**    | 29333 (15.63%) | 29377 (15.66%) | 128931 (68.71%) |
|     Pneumothorax     | 17313 (9.23%)  |  2663 (1.42%)  | 167665 (89.35%) |
| **Plueral Effusion** | 75696 (40.34%) |  9419 (5.02%)  | 102526 (54.64%) |
|    Pleural Other     |  2441 (1.3%)   |  1771 (0.94%)  | 183429 (97.76%) |
|       Fracture       |  7270 (3.87%)  |  484 (0.26%)   | 179887 (95.87%) |
|   Support Devices    | 105831 (56.4%) |  898 (0.48%)   | 80912 (43.12%)  |


##### Some Comments on Public Datasets

+ see [[NIH-chestX14-vs-stanford-chestxpert]] for detailed review
+ Unusable for real produts

---

#### **Conclusions**

+ All three datasets are not too useful as it is
+ We will need to go through all reports manually and relabel them
+ Standford data is easiest to work with
+ We need **500GB** 🙄 of minimum storage to get all of the data!
+ NIH data is too low quality hence is only 42 GB
+ MIT data is very hard to get
+ **Likely Thing to do** - Follow one of papers and repeat them for a subset of tasks on stanford data



