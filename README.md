# Flask AWS Docker Deployment Sample

This is a sample Flask app deployed on AWS EC2 using Docker.  
Run it locally with:

```bash
docker build -t flask-app .
docker run -p 5000:5000 flask-app


### Step 1

Create the Project Structure
flask-aws-docker/
├── app.py
├── Dockerfile
├── requirements.txt
├── README.md

### Step 2

Create a new repo in GitHub and push the files

```bash
git init
git add .
git commit -m "Initial commit - Flask app with Docker"
git remote add origin https://github.com/tokitaohma07/flask-aws-docker.git
git push origin master


### Step 3

Create an Ec2 instance, ubutnu
Custom TCP rule: port 5000(for flask)

### Step 4

Install Docker on EC2

```bash
sudo apt update
sudo apt install docker.io -y
sudo systemctl start docker
sudo usermod -aG docker ubuntu


### Step 5

Cloning GitHub repo to Ec2

```bash
git clone https://github.com/your-username/flask-aws-docker.git


### Step 6

Build and run container

```bash
docker build -t flask-app .
docker run -d -p 5000:5000 flask-app


