# ✅ Day 14 – CI/CD Project (GitHub Actions)

## 📌 What I Did

- Created a Dockerized Flask application (`app.py`)
- Wrote a `Dockerfile` to containerize the app
- Created a GitHub Actions pipeline in `.github/workflows/docker-ci.yml`
- Added secrets (`DOCKER_USERNAME` and `DOCKER_PASSWORD`) securely to GitHub
- Logged in to Docker Hub via GitHub Actions
- Built and pushed the Docker image automatically

---

## 🔧 Workflow File (`docker-ci.yml`)

```yaml
name: Docker CI

on:
  push:
    branches: [ main ]

jobs:
  docker:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v3

      - name: Log in to Docker Hub
        run: echo "${{ secrets.DOCKER_PASSWORD }}" | docker login -u ${{ secrets.DOCKER_USERNAME }} --password-stdin

      - name: Build Docker image
        run: docker build -t ${{ secrets.DOCKER_USERNAME }}/devops-cicd-project:latest .

      - name: Push to Docker Hub
        run: docker push ${{ secrets.DOCKER_USERNAME }}/devops-cicd-project:latest

🐳 Docker Image Details

Image Name: yashyernal/devops-cicd-project
Tag: latest
Registry: Docker Hub

---

🧠 What I Learned

How to securely manage credentials with GitHub Secrets
How to automate Docker workflows using GitHub Actions
How CI/CD pipelines help with continuous delivery
How to troubleshoot YAML and login/push issues
---

✅ Successfully completed the GitHub Actions side of Day 14!