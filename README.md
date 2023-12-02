# Kidney-Microvasculature-Segmentation-and-Prediction-with-YOLO-v8

Overview

This repository contains code for the Kidney Microvasculature Segmentation Challenge. The goal of this task is to develop a model that accurately locates microvasculature structures (blood vessels) within human kidney histology slides. The dataset consists of tiles extracted from Whole Slide Images (WSI) and is split into three datasets: Dataset 1 with expert-reviewed annotations, Dataset 2 with sparse annotations, and Dataset 3 with unannotated tiles for potential semi- or self-supervised learning.

Training Data:

Dataset 1: Tiles with expert-reviewed annotations.

Dataset 2: Tiles with sparse annotations that have not been expert-reviewed.

Dataset 3: Unannotated tiles for potential semi- or self-supervised learning.

Test Data:

Dataset 1 tiles with annotations from the public test set.

Hidden private test set tiles with expert-reviewed annotations.

Evaluation:

Predict blood vessel masks on the test set. False positives within glomerulus structures will be counted.

Files and Field Descriptions

train/test/: Folders containing TIFF images of tiles. Each tile is 512x512 in size.

polygons.jsonl: Polygonal segmentation masks in JSONL format for Dataset 1 and Dataset 2.

tile_meta.csv: Metadata for each image, including source WSI, location, dataset, and more.

wsi_meta.csv: Metadata for the Whole Slide Images, including demographic information about the tissue donor.

