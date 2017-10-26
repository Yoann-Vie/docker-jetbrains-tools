# Docker environment

#### Build and up containers
```
sudo docker-compose up -d --build
```
#### Stop containers
```
sudo docker-compose stop
````
#### Start containers
```
sudo docker-compose start
```
#### Enter in a specific container
```
docker exec -it <container_id> sh
```
#### Leave a container
```
exit
```
---
## JetBrains containers

### UpSource container
For the first build, execute the following commands
```
mkdir -p -m 750 <path to data directory> <path to logs directory> <path to conf directory> <path to backups directory>
sudo chown -R 13001:13001 <path to data directory> <path to logs directory> <path to conf directory> <path to backups directory>
```
If you use the default docker-compose.yml` file, use directly
```
cd <path_to_docker_jetbrains_tools_folder>
mkdir -p -m 750 upsource/data upsource/logs upsource/conf upsource/backups
sudo chown -R 13001:13001 upsource
```

