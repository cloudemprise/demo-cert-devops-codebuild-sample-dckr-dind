# demo-cert-devops-codebuild-sample-dckr-dind

> AWS CodeCommit / GitHub Repository used for the Hands-On Demonstrations in connection with the AWS Certified DevOps Engineer Professional Exam Study course.

![](https://codebuild.eu-central-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiM1NnR0hsUVBaYmVEZ1dibzVvSGNTanNJU1lGcG51eEQ3bmxaSnZ4SjZUL3VCTXN4YWMxa292YWhSOTZyN0p6UUJKckMvMklCaXV5dUxoMEJSbHhldGFzPSIsIml2UGFyYW1ldGVyU3BlYyI6Ing0KzU5KytQa1A2c3M2UDYiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main)

***

This repository contains a CodeBuild project that builds a custom Docker image using the "Docker-In-Docker" **docker:dind** image, i.e. running a Docker container inside Docker to build a custom image. Thus CodeBuild environment must be configured in Privileged Mode.

**Reference:**

AWS CodeBuild - [Docker in custom image sample for CodeBuild](https://docs.aws.amazon.com/codebuild/latest/userguide/sample-docker-custom-image.html)

AWS CodeBuild - [Create a build project: Privileged Environment](https://docs.aws.amazon.com/codebuild/latest/userguide/create-project-console.html#create-project-console-environment)

Docker CLI - [Runtime privilege and Linux capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities)

DockerHub - [Docker-in-Docker](https://hub.docker.com/_/docker/)

Docker Storage - [Use the OverlayFS storage driver](https://docs.docker.com/storage/storagedriver/overlayfs-driver/)
