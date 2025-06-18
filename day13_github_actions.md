# ✅ Day 13 – GitHub Actions CI/CD

## 📌 What I Did
- Learned the fundamentals of GitHub Actions
- Created `.github/workflows/ci.yml` for automated CI
- Used GitHub-hosted runners to run shell commands
- Added a custom script (`greeting.sh`) as a pipeline step
- Verified successful execution in the GitHub Actions UI

---

## 🔧 Workflow: `.github/workflows/ci.yml`

```yaml
name: Day 13 CI Workflow

on:
  push:
    branches:
      - main

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Print welcome message
        run: echo "✅ GitHub Actions pipeline running..."

      - name: List project files
        run: ls -l

      - name: Give execute permission to greeting.sh
        run: chmod +x greeting.sh

      - name: Run greeting.sh script
        run: ./greeting.sh

📜 Script: greeting.sh


#!/bin/bash
echo "👋 Hello from Day 13 – GitHub Actions CI/CD!"

🧠 What I Learned

GitHub Actions YAML structure
Triggering jobs on push events
Running custom shell scripts
Viewing logs & build steps in the Actions tab

🧰 Tools Used
GitHub
GitHub Actions
YAML
Shell scripting

✅ Successfully completed Day 13 of the DevOps 30-Day Journey 🚀

yaml
Copy
Edit
