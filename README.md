# demo-cert-devops-codebuild-sample-dckr-dind

> AWS CodeCommit / GitHub Repository used for the Hands-On Demonstrations in connection with the AWS Certified DevOps Engineer Professional Exam Study course.

![](https://codebuild.eu-central-1.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiazhSSEZCeE1RSUowM3lUVTUyd0lZMDFGYlMzaEl1c1QycGpRRFVSNll3bkVtUTdoQWN6Y2RKc1ZaMjN4RlE2MjVDeUZUNzJwamdDTm5uVVlRbCsxT1lJPSIsIml2UGFyYW1ldGVyU3BlYyI6IjVKalRJc1RpVGlrZXZlbzEiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=main)

***

This repository contains a AWS CodeBuild project that builds a Docker image using a Custom Docker Image as apposed an image that is managed and supplied by AWS CodeBuild. The build Custom Docker Image that is used is an official DockerHub release refered to as the "Docker-In-Docker" image, i.e. **docker:dind** . In other words what we are doing here is running the Docker Engine inside a Docker container which is then used to build a custom image.

Note: The CodeBuild project environment must be configured in Privileged Mode.

**Reference:**

- AWS CodeBuild - [Docker in custom image sample for CodeBuild](https://docs.aws.amazon.com/codebuild/latest/userguide/sample-docker-custom-image.html)

- DockerHub - [Docker-in-Docker](https://hub.docker.com/_/docker/)

- AWS CodeBuild - [Create a build project: Privileged Environment](https://docs.aws.amazon.com/codebuild/latest/userguide/create-project-console.html#create-project-console-environment)

- Docker CLI - [Runtime privilege and Linux capabilities](https://docs.docker.com/engine/reference/run/#runtime-privilege-and-linux-capabilities)


- Docker Storage - [Use the OverlayFS storage driver](https://docs.docker.com/storage/storagedriver/overlayfs-driver/)
