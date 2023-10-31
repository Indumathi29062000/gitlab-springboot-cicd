# Sample Spring Boot Application Deployment with GitLab CI/CD

This repository shows my experience in deploying a simple Spring Boot application using GitLab CI/CD.
The application is built, tested, packaged, and deployed to Docker Hub following the steps below:

## Steps:

1. **Project Creation:**
   - created a Spring Boot application for this project.

2. **Import to GitLab:**
   - imported the project into GitLab from this github repository

3. **GitLab CI/CD Setup:**
   -  utilized the GitLab Pipeline Editor to create a `.gitlab-ci.yml` file for the CI/CD pipeline.

4. **Define Stages:**
   - In the `.gitlab-ci.yml` file, I defined the following stages:
     - `build`:  used Maven for the build stage.
     - `test`: ran Maven tests.
     - `package`: packaged the application.
     - `docker-image`: created a Docker image using a Dockerfile.
     - `docker-container`: deployed the Docker image to Docker Hub.

5. **Docker Image Setup:**
   -  created a Dockerfile to build a Docker image for the Spring Boot application.

6. **GitLab CI/CD Pipeline:**
   - observed that the GitLab CI/CD pipeline automatically triggers when changes are pushed to the repository.

7. **Pipeline Success:**
   - ensured that the pipeline completes successfully, which includes:
     - Successful Maven build and test stages.
     - Building a Docker image.
     - Pushing the Docker image to Docker Hub.

8. **`.gitlab-ci.yml` Configuration:**
   - The pipeline configuration in the `.gitlab-ci.yml` file uses stages, jobs, and Docker images for building, testing, and deploying.

9. **Docker Hub Credentials:**
   - configured Docker Hub credentials in my GitLab project to securely push the Docker image to Docker Hub, using environment variables for this purpose.

10. **Docker Image Deployment:**
    -  successfully pushed the Docker image to Docker Hub, making it available for others to use for container deployment.

## Conclusion:

The automation of the build, test, and deployment processes simplifies the management and sharing of the application using Docker containers. below is the screenshot of gitlab pipeline:
![image](https://github.com/Indumathi29062000/gitlab-springboot-cicd/assets/77050907/9a95c3cb-f291-45be-8d72-b6595f1b8f12)

