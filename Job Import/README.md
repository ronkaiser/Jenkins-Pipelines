# Job Import Pipeline 

## Description 
In this pipeline we are going to transfer job1 environment variables into job2 pipeline. 

### Preparation steps: 
- Install `job import` plugin. 
- Define job1 with Jenkinsfile as `Jenkinsfile-trigger`.
  Notice that in this example the parameter is `image_build` which hold `BUILD_NUMBER` variable of job1. 
- Define job2 and check `This project is parameterized`. 
- In `Name` define the same name of parameter from job1. 
- select `Name` and `Default Value` such as `$BUILD_NUMBER`. 

### Build:
- Click on `Build now` in job1
- If job2 for example will echo BUILD_NUMBER, it will print the build number of job1. 