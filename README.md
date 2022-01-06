# demo-cert-devops-codebuild-sample-dckr-dind

> AWS CodeCommit / GitHub Repository used for the Hands-On Demonstrations in connection with the AWS Certified DevOps Engineer Professional Exam Study course.

![](https://codebuild.eu-central-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiazhSSEZCeE1RSUowM3lUVTUyd0lZMDFGYlMzaEl1c1QycGpRRFVSNll3bkVtUTdoQWN6Y2RKc1ZaMjN4RlE2MjVDeUZUNzJwamdDTm5uVVlRbCsxT1lJPSIsIml2UGFyYW1ldGVyU3BlYyI6IjVKalRJc1RpVGlrZXZlbzEiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main)

***

This repository contains artifacts related to an AWS CodeBuild project and its auxillary components. These components build a Docker image using a 'Custom Docker Image' as apposed an image that is managed and supplied by the AWS CodeBuild service. The build 'Custom Docker Image' that is used is an official DockerHub release refered to as the "Docker-In-Docker" image, i.e. **docker:dind** . In other words what we are doing here is running the Docker Engine inside a Docker container which is then used to build a custom Docker image.

Also, documented here is a bash script highlighting useful API calls that relate to the AWS CodeBuild service in connection with this exercise as well as an AWS CloudFormation infrastructure template describing all the important AWS resources.

Note: 

- The CodeBuild project environment must be configured in Privileged Mode.
- Custom image > Environment type = Linux > Image registy = Other registry > External registry URL = docker:dind

**Reference:**

- AWS CodeBuild - [Docker in custom image sample for CodeBuild](https://docs.aws.amazon.com/codebuild/latest/userguide/sample-docker-custom-image.html)

- DockerHub - [Docker-in-Docker](https://hub.docker.com/_/docker/)

- AWS CodeBuild - [Create a build project: Privileged Environment](https://docs.aws.amazon.com/codebuild/latest/userguide/create-project-console.html#create-project-console-environment)

- Docker CLI - [Runtime privilege and Linux capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities)

- Docker Storage - [Use the OverlayFS storage driver](https://docs.docker.com/storage/storagedriver/overlayfs-driver/)


> **Relavent APIs:**

> [create-project](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/codebuild/create-project.html)

> [list-projects](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/codebuild/list-projects.html)

> [batch-get-projects](https://awscli.amazonaws.com/v2/documentation/api/latest/reference/codebuild/batch-get-projects.html)
