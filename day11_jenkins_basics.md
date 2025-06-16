# ✅ Day 11 – Jenkins Basics

## 📌 What I Did
- Installed Jenkins using Docker:
  ```bash
  docker run -d -p 8080:8080 -p 50000:50000 --name jenkins -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts

  Accessed Jenkins UI at http://localhost:8080 (via Play with Docker)

Unlocked Jenkins using the initial admin password
Installed suggested plugins
Created the first admin user
Set up and ran a Freestyle project

🔧 Jenkins Job Details

Job Name:
my-first-job

Build Steps:
Shell command:

echo "Jenkins job executed successfully"
echo "Cloned repo successfully"
ls -l


Git Integration:
Repo: https://github.com/yash1206yernal/devops-week1-mini-project

Branch: main
Jenkins successfully cloned the repo and ran the build script.

✅ Output Highlights:

Jenkins console output confirmed:

Jenkins job executed successfully
Cloned repo successfully
README.md
welcome.sh

Final build result: SUCCESS

🧠 What I Learned

Jenkins installation via Docker
Initial setup and plugin configuration
Creating and configuring Freestyle jobs
Pulling code from GitHub
Automating basic shell scripts using Jenkins

📚 Tools Used

Jenkins
Docker
GitHub
