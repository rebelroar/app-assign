### Prerequisites
- Docker
- Docker Compose
- Jenkins

### Running Locally
1. Clone the repository:
   ```git clone https://github.com/yourusername/MyApp.git```
   ```cd MyApp```

2. Build Images
- docker build -t rebelroar/go-app ./go-app
- docker build -t rebelroar/nextjs-app ./nextJS-app
- docker build -t rebelroar/wordpress-app ./wordpress-app

3. Push images
- docker push rebelroar/go-app
- docker push rebelroar/nextjs-app
- docker push rebelroar/wordpress-app


### Orchestration
1. Deploying with docker compose
- docker-compose up


### Deploying in GCP App Engine
For this I am storing my image at GCR registry and deploying app in Cloud Run.
I have written Jenkinsfiles for all three components. When we run these Jenkinsfiles from Jenkins these applications on Cloud Run.
