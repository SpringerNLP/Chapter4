# Chapter 4 - Basics of Deep Learning Case Study
This case study explores the basics of deep learning. In the first portion of the case study, training of a neural network is performed with a numpy implementation, then we explore supervised and unsupervised techniques on a [spoken digit](https://github.com/Jakobovski/free-spoken-digit-dataset) recognition task. 

## Requirements
Without GPU (CPU only):
* [Docker](https://docs.docker.com/install/) 

If using a GPU: 
* [Nvidia docker2](https://github.com/nvidia/nvidia-docker/wiki/Installation-(version-2.0)#installing-version-20)

## Running the Docker Image
The docker images for this case study are located on dockerhub. Running the commands below will automatically download and start a jupyter notebook.

Run the Docker image for CPU only computation:
```
docker run -p 8888:8888 --rm springernlp/chapter_4:latest
```

Run the Docker image with GPU access: 
```
docker run --runtime=nvidia -p 8888:8888 --rm springernlp/chapter_4:latest
```

## Building the Docker image
```
docker build -t chapter_4:latest .
```
