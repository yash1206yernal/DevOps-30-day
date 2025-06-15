# ✅ Day 10 – Docker Project

## 🧱 App Description
- Built a Python Flask web app that logs every visit to `logs/app.log`
- Displays a message: "✅ Hello from Dockerized Flask App!"
- Persisted logs using Docker volume

## 🐳 Docker Setup
- Used a custom `Dockerfile` to install Flask and run the app
- Mounted local `logs/` directory to container for persistence
- Exposed port 5000 to access via browser

## 🧩 Docker Compose
- Managed the app with `docker-compose.yml`
- Simplified building and running with:
  ```bash
  docker-compose up --build
  docker-compose down
🧪 Commands Used

docker build -t my-python-app .
docker-compose up --build
docker-compose down
cat logs/app.log

💡 What I Learned

How to containerize a Python app
Build and run images using Dockerfile
Use volumes to persist app logs
Use Docker Compose to orchestrate multi-container apps
