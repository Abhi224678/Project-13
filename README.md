# Project 13: Build Image and Push to Amazon ECR

## Objective

To build a Docker image and publish it to Amazon Elastic Container Registry (ECR).

## Tools Used

- Linux VM (Ubuntu)
- Docker
- AWS CLI
- Amazon ECR
- AWS IAM

## Implementation Steps

1. Created a separate project directory for Project 13.
2. Created a Dockerfile using the lightweight `nginx:alpine` base image.
3. Verified AWS CLI authentication using `aws sts get-caller-identity`.
4. Checked the AWS region (`ap-south-1`).
5. Used the existing ECR repository named `project13-app`.
6. Built the Docker image using Docker.
7. Tagged the image with the ECR repository URI.
8. Authenticated Docker with Amazon ECR using AWS CLI.
9. Pushed the Docker image to the ECR repository.
10. Verified the uploaded image using the AWS CLI `list-images` command.

## AWS ECR Details

- **AWS Account ID:** 590507089733
- **Region:** ap-south-1 (Mumbai)
- **Repository Name:** project13-app
- **Image Tag:** latest

## Docker Commands Used

### Build Docker Image

```bash
docker build -t project13-app .
