# ✅ Day 8 – Docker Basics (via Play with Docker)

## 🔧 Docker Commands Practiced

```bash
docker pull alpine
docker run alpine echo "Hello from Docker!"
docker run -it alpine /bin/sh
docker ps
docker ps -a
docker rm <container_id>
docker rmi alpine

💡 Concepts I Learned
Difference between containers and VMs
Docker containers are fast and lightweight
alpine is a minimal Linux image ideal for testing
How to run one-time and interactive containers
How to clean up containers and images

Enviromets used: Play with Docker
