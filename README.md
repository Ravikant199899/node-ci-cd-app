# 🚀 Node.js CI/CD Pipeline with GitHub Actions & Docker

## 🎯 Objective
Automate the build, test, and deployment of a **Node.js web application** using **GitHub Actions** and **DockerHub**.  
This project demonstrates a complete **CI/CD pipeline** for containerized applications.

---

## 🛠 Tools Used
- **GitHub** (repository & workflows)
- **GitHub Actions** (CI/CD automation)
- **Node.js** (application runtime)
- **Docker** & **DockerHub** (containerization & image registry)

---

## 📂 Project Structure

node-ci-cd-app/
│── .github/
│ └── workflows/
│ └── main.yml # CI/CD pipeline definition
│── Dockerfile # Builds the Node.js app container
│── index.js # Main application entry point
│── package.json
│── package-lock.json
│── dummy.txt # Placeholder/test file
└── README.md # Project documentation


---

## ⚙️ CI/CD Workflow (`main.yml`)

Triggered on every push to the **main** branch:

1. **Checkout** repository code
2. **Install dependencies** (Node.js)
3. **Run tests** (if present)
4. **Build Docker image**
5. **Authenticate** with DockerHub using **GitHub Secrets**
6. **Push image** to DockerHub

---

## ▶️ How to Reproduce

1. Clone the repo:
   ```bash
   git clone https://github.com/Ravikant199899/node-ci-cd-app.git
   cd node-ci-cd-app
   ```
2 Ensure you have:

** .github/workflows/main.yml

** Dockerfile

** index.js, package.json, etc.

3. Push any change to the main branch — GitHub Actions will trigger automatically.

Verify:

** Build status in Actions tab

** Image pushed to DockerHub

4. Run locally:
 ```bash
   docker pull <your-dockerhub-username>/node-ci-cd-app:latest
docker run -p 3000:3000 <your-dockerhub-username>/node-ci-cd-app:latest
```

📘 Learning Outcomes

Built a working CI/CD pipeline with GitHub Actions

Automated Docker image build & push

Gained hands-on skills in continuous integration & deployment for Node.js apps

👤 Author

Ravikant Jadhav
