# Brain_Tumor_Detection

This repository contains a deep learning model for detecting brain tumors using medical imaging. The model is trained using YOLOv8 and Detr-Resnet-101.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)

## Overview

The goal of this project is to provide an automated solution for detecting brain tumors in medical images. The model is trained using a dataset of brain MRI images and can classify tumors into the following categories:

- Glioma
- Meningioma
- No Tumor
- Pituitary

## Installation

To get started, clone this repository and set up the environment.

`pip install -r requirements.txt`

## Usage

Place the trained Yolov8 and Detr-Resnet-101 models in model folder.

Run the app with following command.
`python app.py`

## Folder Structure
Brain_Tumor_Detection/
│
├── datasets/
│   └── test/
│       ├── images/
│       └── labels/
│
├── model/
│   └── detr_resnet_101/
│       └── DETR_model/
|           ├── config
|           └── model.safetensors
|   └── yolov8
|       └──best.pt
│
├── static/
│   └── css/
│       └── styles.css
│
├── templates/
│   ├── index.html
│   └── predict.html
│
├── brain_tumor_probs.py
├── brain_tumor_visual.py
├── detr_model.py
├── README.md
└── requirements.txt
