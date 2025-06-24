**# Flask Docker App on AWS EC2**

This is a simple Python Flask web application, containerized using Docker, and deployed on an AWS EC2 instance.

**## 🚀 Features**

- Flask web app (`app.py`)
- Dockerized using a custom `Dockerfile`
- Deployable on any server (tested on AWS EC2)
- Lightweight image using `python:3.10-slim`

**## 🛠️ Requirements**

- Python 3.x
- Docker
- AWS EC2 instance (Ubuntu or Amazon Linux 2)

**## 📁 **Project Structure****

flask-docker-app/
├── app.py
├── requirements.txt
├── Dockerfile
└── README.md


**## 📦** Build and Run Locally****

```bash
docker build -t flask-app .
docker run -p 5000:5000 flask-app

Access the app at **http://localhost:5000**

☁️ **Deploy on AWS EC2**
1. Launch an EC2 instance
2. SSH into the instance and install Docker
3. Clone this repo or create the files directly
4. Run:
        docker build -t flask-app .
        docker run -d -p 5000:5000 flask-app
5. Visit: **http://<your-ec2-public-ip>:5000**
