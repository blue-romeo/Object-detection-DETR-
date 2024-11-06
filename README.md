# Hardhat Detection with DETR

This project demonstrates how to fine-tune a DETR (Detection Transformer) model for hardhat detection using the Hugging Face Transformers library.

## Overview

The goal of this project is to build a real-time hardhat detection system. This is achieved by fine-tuning a pre-trained DETR model on a hardhat dataset. The model can then be used to detect persons and whether they are wearing a helmet or not in real-time.

## Dataset

The project uses the `anindya64/hardhat` dataset from Hugging Face Datasets. This dataset contains images of construction workers, some of whom are wearing hardhats. The dataset is preprocessed to match the format expected by the DETR model.

## Model

The project uses the `facebook/detr-resnet-50-dc5` model from Hugging Face Model Hub. This model is a pre-trained DETR model that has been fine-tuned on the COCO dataset. The model is further fine-tuned on the hardhat dataset to improve its performance on hardhat detection.

## Training

The model is trained using the Hugging Face Trainer. The training process involves the following steps:

1. Loading the base (pre-trained) model.
2. Defining the training hyperparameters.
3. Passing the training arguments to the Trainer.
4. Calling the `train()` method to fine-tune the model.

## References

* [Hugging Face Transformers](https://huggingface.co/transformers/)
* [Hugging Face Datasets](https://huggingface.co/datasets/)
* [Hugging Face Model Hub](https://huggingface.co/models/)
