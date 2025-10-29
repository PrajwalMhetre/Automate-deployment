# Automate-deployment
Automate full deployment of a web app using:  Jenkins for CI/CD pipeline (build → test → deploy)  Terraform for cloud infrastructure automation (AWS / Azure / GCP)  Everything containerized with Docker
Developer Pushes Code → GitHub
        ↓
     Jenkins CI/CD
        ↓
Build App with Docker → Push Image to DockerHub
        ↓
Trigger Terraform → Provision Cloud Infrastructure
        ↓
Terraform deploys container on EC2 / GKE / AKS
        ↓
Send Slack/Email Notification of Successful Deploy
