# Docker-Practice
This is a simple Docker Project which performs following tasks.
- `Pull` docker  `Nginx` image from `docker Hub`
- `Create` docker container with this `Nginx` image
- `Copy` all files from current directory & paste into the container
- `Run` docker container on `port 5000` with our application

 
## Requirements
1. `Docker`
  ```
  yum install docker (Amazon Linux/fedora/CentOS)
  apt install docker.io (Ubuntu/Debian)
  ```

## Installation
1. Clone the repository
  ```
  https://github.com/Ujwal-s-Projects/Docker-Practice.git
  ```

2. Enter into main directory
  ```
  cd Docker-Practice/
  ```

3. Create docker Image
  ```
  docker build -t my-app:latest .
  ```

4. Run docker container in daemon mode/background
  ```
  docker run -d --name my-con -p "5000:80" my-app:latest 
  ```

5. Copy `Public IP` and paste it in the browser to access the application
  ```
  http://<public_ip>:5000
  ```


