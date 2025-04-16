# Flask AWS Docker Deployment Sample

This is a sample Flask app deployed on AWS EC2 using Docker.  
Run it locally with:

```bash
docker build -t flask-app .
docker run -p 5000:5000 flask-app
