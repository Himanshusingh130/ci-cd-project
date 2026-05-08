# CI/CD Pipeline Using GitHub Actions, Docker & Jenkins

## Technologies Used
- GitHub Actions
- Docker
- Jenkins
- Node.js
- Express.js

## Run Locally

### Install Dependencies
```bash
npm install
```

### Start Application
```bash
npm start
```

### Docker Build
```bash
docker build -t app-ci .
```

### Run Docker Container
```bash
docker run -d -p 3000:3000 app-ci
```

## CI/CD Workflow
Code Push → GitHub Actions → Docker Build → Docker Hub → Jenkins Deployment
