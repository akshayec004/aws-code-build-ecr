# aws-code-build-ecr
## Building docker image with CodeBuild and pushing it to ECR
- buildspec.yml - Specification file for the CodeBuild. Consists of pre_build, build and post_build phases
- Dockerfile - Docker file for building docker image

Steps to create a docker image and push it to ECR :
* Go to ECR and create a repository. Note down the repository URI
* Update the REPOSITORY_URI to the one noted in the step 2.
* Go to the CodeBuild and create a project. Make sure the role attached to the project has the permission to access the ECR.
* Build the project and check in the ECR if the image is pushed or not.
