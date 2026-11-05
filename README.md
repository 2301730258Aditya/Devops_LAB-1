devops-lab1-ci
ENSP461 - DevOps and Automation, Lab 1: DevOps Foundations & Continuous Integration.

This repo contains a small Flask application used to demonstrate a complete CI/CD workflow with Git, GitHub and Jenkins on Ubuntu 24.04 LTS.

Structure
app/ - Flask application source code
tests/ - pytest unit tests
scripts/ - deployment helper scripts
Jenkinsfile - declarative pipeline (build / test / deploy)
docs/ - command logs, screenshots and observations
reports/ - final lab report PDFs
Run locally
python3 -m venv venv source venv/bin/activate pip install -r app/requirements.txt python -m flask --app app.app run

Pipeline
Checkout from GitHub
Build (install dependencies)
Test (pytest)
Deploy (systemd service + health check)
