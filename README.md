# Jenkins CI/CD Node.js Demo 🚀

This project demonstrates a simple CI/CD pipeline using Jenkins to build and deploy a Node.js app.

## 🔧 Tech Stack
- Node.js (Express)
- Jenkins (running via Docker)
- Declarative Pipeline (`Jenkinsfile`)

## 🛠️ Features
- Auto build on push
- Stages: Build → Test → Deploy
- Jenkinsfile defines pipeline steps

## 📦 Setup & Run Locally

```bash
# Clone the repo
git clone https://github.com/AbrarKivande/jenkins-demo-app.git
cd jenkins-demo-app

# Start the app locally (optional)
npm install
npm start

🚀 Jenkins Setup (via Docker)

# Create a Docker network
docker network create jenkins-net

# Run Jenkins container
docker run -d --name jenkins \
  -p 8080:8080 -p 50000:50000 \
  --network jenkins-net \
  -v jenkins_home:/var/jenkins_home \
  jenkins/jenkins:lts

Access Jenkins at http://localhost:8080

Made with ❤️ by Abrar Kivande