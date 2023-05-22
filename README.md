# python-application
# Deploy python-application with Docker
# Pre-Requisites

- Git
- Docker

# Docker Build & Push
- docker build -t naresh240/python-ecs:latest .
- docker login
- docker push naresh240/python-ecs:latest
# Deploy Application using Docker Run Command
docker run --name python-ecs-container -p 5000:5000 -d naresh240/python-ecs:latest

# Check running containers
- docker ps -a
# Clean UP
- docker stop <container-ID>
- docker rm <container-ID>
