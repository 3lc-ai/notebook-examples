# TLC Python Package Example Notebooks

Welcome to our collection of example notebooks for the `tlc` Python package! This repository contains various Jupyter
notebooks that demonstrate how to use the `tlc` Python package across different scenarios and use cases.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing
purposes.

### Prerequisites

You will need the following tools installed on your system:

+ A suitable version of Python (See [documentation](https://docs.3lc.ai/3lc/2.2/quickstart/quickstart.html#requirements) for supported versions)
+ Access to the `tlc` Python package

### Installation

Clone this repository to your local machine:

```bash
# Copy code
git clone https://github.com/3lc-ai/notebook-examples.git

# Navigate to the cloned directory:
cd notebook-examples

# Activate your Python environment (if applicable)

# Open the Jupyter notebook interface:
jupyter notebook

#From the Jupyter interface, open any notebook from the list to get started.
```

## Notebooks Overview

Here's a brief overview of the example notebooks included in this repository:

+ [MNIST](./pytorch-mnist.ipynb): Train a simple model on the MNIST dataset and collect classification metrics.
+ [CIFAR-10](./pytorch-cifar10.ipynb): Train a model on the CIFAR10 dataset and collect classification metrics.
+ [Hugging Face IMDB Reviews](./huggingface-imdb.ipynb): Use our Hugging Face `Trainer` integration to train a language
  model on the IMDB Reviews dataset.
+ [Hugging Face CIFAR-100](./huggingface-cifar100.ipynb): Loads the CIFAR-100 dataset from Hugging Face dataset
  and computes dimensionality reduced 2D image embeddings.
+ [Detectron2 Balloons](./detectron2-balloons.ipynb): Trains an object detection model and gathers bounding box metrics
  with detectron2.
+ [Detectron2 COCO128](./detectron2-coco128.ipynb): Executes inference and gathers bounding box metrics using
  detectron2.
+ [Per Bounding Box Metrics](./calculate-luminosity.ipynb): Describes metric collection for individual bounding boxes in
  images.
+ [Per Bounding Box Embeddings](./add-bb-embeddings.ipynb): Covers embedding collection for bounding boxes and uses UMAP
  for dimensionality reduction.
+ [Bounding Box Classifier](./train-bb-classifier.ipynb): Details an advanced workflow where a model is trained to
  classify bounding boxes in an image, which can be used in conjunction with an object detection model to find bounding
  boxes of special interest.
+ [PyTorch Lightning SegFormer](./pytorch-lightning-segformer.ipynb): Demonstrates how to use a custom metrics collector
  for collecting predicted masks from a semantic segmentation model.

Each notebook is self-contained and declares and installs its required dependencies.

### Data

All required data for running the notebooks is either contained in the `./data` folder, or is downloaded from the internet during the notebook execution.

## Contributing

We welcome contributions to this repository! If you have a suggestion for an additional example or improvement, please open an issue or create a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

We use two versions of the Balloons dataset:

**Title**: Balloons Dataset  
**Author**: Paul Guerrie  
**Publisher**: Roboflow  
**Year**: 2024  
**URL**: [Balloons Dataset on Roboflow Universe](https://universe.roboflow.com/paul-guerrie-tang1/balloons-geknh)  
**Note**: Visited on 2024-03-15

**Title**: Mask R-CNN for object detection and instance segmentation on Keras and TensorFlow  
**Author**: Waleed Abdulla  
**Year**: 2017  
**Publisher**: Github  
**URL**: [Releases](https://github.com/matterport/Mask_RCNN/releases)  
**Repository**: [GitHub repository](https://github.com/matterport/Mask_RCNN)

We also use the first 128 images from the [COCO](https://cocodataset.org/#home) dataset.
