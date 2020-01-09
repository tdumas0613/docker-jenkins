# docker-jenkins
An extension of the official Docker image for Jenkins

- Usage:
  - Build Command: docker build -t {imageName}:{imageTag} /path/to/Dockerfile
  - Run Command: docker run -p 8080:8080 -v jenkins_home:/var/jenkins_home -d {imageName}:{imageTag}
    - -d runs in detached mode
    - -v uses persistant volume to load jenkins configuration
    - -p port to access Jenkins at
  - Access at localhost:8080 (or port 8080 at whatever IP Address instance is running at)
  
  - More information can be found at https://github.com/jenkinsci/docker/blob/master/README.md
