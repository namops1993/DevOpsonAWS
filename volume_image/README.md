## 1. Command

docker volume create mysql_vo
docker pull mysql:5.6
docker run -d --name some-mysql -v mysql_vo:/var/lib/mysql  -e MYSQL_ROOT_PASSWORD=devops_pw  mysql:5.6


## 2. Command to run mount file

docker build -t test_vo -f Dockerfile2 .

docker run -v /Users/namnh68/FGit/DevOpsOnAWS_Training/volume_image/devops.txt:/app/devops.txt test_vo

## 3. Command to run mount file

docker build -t test_vo -f Dockerfile3 .

docker run -v /Users/namnh68/FGit/DevOpsOnAWS_Training/volume_image:/app/ test_vo
