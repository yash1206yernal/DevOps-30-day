# ✅ Day 12 – Jenkins Pipelines

## 📌 What I Did
- Learned the difference between Freestyle Jobs and Pipeline Jobs
- Created a **Pipeline Job** in Jenkins
- Wrote and ran a **Declarative Jenkinsfile**
- Configured Jenkins to pull a `Jenkinsfile` from a **GitHub repo**
- Successfully executed a multi-stage pipeline

---

## 🧱 Jenkinsfile Structure

Created a Jenkinsfile with 3 stages:

```groovy
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '🔨 Building from GitHub repo...'
            }
        }
        stage('Test') {
            steps {
                echo '✅ Testing from GitHub repo...'
            }
        }
        stage('Deploy') {
            steps {
                echo '🚀 Deploying from GitHub repo...'
            }
        }
    }
}

🧩 Job Details

Job Type: Pipeline
SCM Configured: GitHub
Repository: https://github.com/yash1206yernal/devops-week1-mini-project
Branch: main
---

🔄 Execution Log

Sample output in Console:

🔨 Building from GitHub repo...
✅ Testing from GitHub repo...
🚀 Deploying from GitHub repo...
Finished: SUCCESS

---

🧠 What I Learned

How to define pipelines as code using Jenkinsfile
How to version and manage CI/CD workflows through GitHub
How Jenkins interacts with Git repositories
Difference between inline pipeline and SCM-based pipeline

---
🧰 Tools Used

Jenkins
GitHub
Docker
Declarative Pipeline Syntax
