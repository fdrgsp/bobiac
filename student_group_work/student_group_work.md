# <i class="fa-solid fa-user-group"></i> Student Group Work

## Overview

Your turn! The goal of this group work is to apply the knowledge you have acquired in the course to develop a cell (instance) segmentation pipeline on 2D images provided.

## Data

<a href="../_static/data/student_group_work/001_img.tiff" download> <i class="fas fa-download"></i> Student Group Work Image </a>

## Submission

To submit your results, use the following notebook: [Evaluation notebook](../../notebooks/student_group_work/evaluation-notebook.ipynb)


## Leaderboard

The leaderboard is available at [BoBIAC 2025 Segmentation Leaderboard](https://liveboard-bobiac.onrender.com/).

## Evaluation metrics

Evaluating segmentation pipelines is a complex task, and there is no single metric that can capture all the aspects of the performance. We have chosen to use the following metrics:

- **Precision**: The precision is the percentage of pixels that are correctly classified.

$$
\text{Precision} = \frac{\text{Number of correctly classified pixels}}{\text{Total number of pixels}}
$$

- **Recall**: The recall is the percentage of pixels that are correctly classified.

$$
\text{Recall} = \frac{\text{Number of correctly classified pixels}}{\text{Total number of pixels in the ground truth}}
$$

- **Intersection over Union (IoU)**: The intersection over union is the ratio of the intersection of the predicted and ground truth masks to the union of the two masks.

$$
\text{IoU} = \frac{\text{Intersection}}{\text{Union}}
$$

- **Pixel accuracy**: The pixel accuracy is the percentage of pixels that are correctly classified.

$$
\text{Pixel accuracy} = \frac{\text{Number of correctly classified pixels}}{\text{Total number of pixels}}
$$

- **Mean Intersection over Union (mIoU)**: The mean intersection over union is the average of the intersection over union for each class.

$$
\text{mIoU} = \frac{1}{n} \sum_{i=1}^{n} \frac{\text{Intersection}_i}{\text{Union}_i}
$$

- **Pixel F1 score**: The pixel F1 score is the harmonic mean of the precision and recall.

$$
\text{Pixel F1 score} = 2 \times \frac{\text{Precision} \times \text{Recall}}{\text{Precision} + \text{Recall}}
$$
