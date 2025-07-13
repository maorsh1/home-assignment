# HelloWorldApp - CI/CD Pipeline

Simple .NET 8 Hello World app with a GitHub Actions pipeline that builds, tests, and deploys using Docker.

## Usage

Clone and run locally:

```bash
git clone https://github.com/maorsh6/HelloWorldApp.git
cd HelloWorldApp
dotnet build
dotnet run

docker build -t maorsh6/hello-world:latest .
docker run --rm maorsh6/hello-world:latest

CI/CD Pipeline
Triggered on push to master. Steps:

Checkout code

Setup .NET 8

Restore, build, test, publish app

Build, scan, push Docker image

Run container to validate output

GitHub Secrets
Add these to your repo settings:

DOCKERHUB_USER: Docker Hub username (maorsh6)

DOCKERHUB_TOKEN: Docker Hub password or token

Created by Maor Sh
Contact me for questions or collaboration.
