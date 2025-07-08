# 🚀 Hello Docker - Simple Node.js App in a Docker Container

This is a beginner-friendly project that demonstrates how to containerize a basic Node.js application using Docker. The app simply runs a server and responds with a message: **"Hello from Docker!"**

## 📦 Tech Stack

- Node.js
- Docker

---

## 📁 Project Structure

hello-docker/
│
├── Dockerfile # Docker build file
├── package.json # Node.js metadata and dependencies
└── server.js # Main application file


---

## 🧑‍💻 Prerequisites

Before running this project, make sure you have:

- [Node.js](https://nodejs.org/) (only needed if running outside Docker)
- [Docker](https://docs.docker.com/get-docker/) installed and running

If you're using an EC2 Ubuntu instance:
```bash
sudo apt update
sudo apt install docker.io -y
sudo systemctl start docker
sudo systemctl enable docker

🚀 How to Run the App with Docker
git clone https://github.com/<your-username>/hello-docker.git
cd hello-docker

docker build -t hello-docker .

docker run -d -p 3000:3000 hello-docker

 🌐 Access the Application
On localhost:
Open your browser and go to: http://localhost:3000

On EC2 instance:
Go to: http://<YOUR_EC2_PUBLIC_IP>:3000

docker ps           # Get container ID
docker stop <CONTAINER_ID>
docker rm <CONTAINER_ID>

