# ✅ Day 9 – Docker Advanced Summary

## 🧱 Dockerfile
- Created a Python file (`app.py`)
- Wrote a Dockerfile to build a custom image
- Used: `FROM`, `WORKDIR`, `COPY`, `CMD`
- Built and ran the image successfully

## 💾 Volumes
- Created named volume: `myvolume`
- Persisted data in `/data/info.txt` across containers
- Verified using Alpine + `cat` command

## 🧩 Docker Compose
- Defined `nginx` + `redis` in `docker-compose.yml`
- Exposed NGINX on port 8080
- Used `docker-compose up` and `down` to manage services

## 🔧 Commands Practiced
```bash
docker build -t my-python-app .
docker run my-python-app
docker run -v myvolume:/data alpine sh -c "echo 'This is saved' > /data/info.txt"
docker run -v myvolume:/data alpine cat /data/info.txt
docker-compose up -d
docker-compose down

🚀 Tools Used
Dockerfile
Docker Volumes
Docker Compose
