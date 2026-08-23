# Movie Picture Pipeline — Submission Evidence

Repository: https://github.com/Dasaridileep/cd12354-Movie-Picture-Pipeline

## Evidence

1. **01_backend_cd_success.png** — Backend Continuous Deployment succeeded: lint and test ran in parallel, followed by Docker build/push and EKS deployment.
2. **02_frontend_cd_success.png** — Frontend Continuous Deployment succeeded: lint and test ran in parallel, followed by Docker build/push and EKS deployment.
3. **03_backend_ci_success.png** — Backend Continuous Integration succeeded: parallel lint/test jobs completed before the Docker build job.
4. **04_frontend_ci_success.png** — Frontend Continuous Integration succeeded: parallel lint/test jobs completed before the Docker build job.
5. **05_kubernetes_runtime_and_backend_api.png** — EKS node is Ready, frontend/backend pods are Running, LoadBalancer services exist, and `/movies` returns the expected JSON.
6. **06_frontend_application.png** — The deployed frontend is reachable and displays all three movies returned by the backend.
7. **07_ecr_images.png** — Both ECR repositories contain deployed images with `latest` and commit-SHA tags.
8. **08_terraform_apply_success.png** — Terraform successfully created the remaining EKS resources and printed the ECR and cluster outputs.

## Deployed Endpoints

- Frontend: http://adef3f05749b242cb81f7052163b8ab3-336861300.us-east-1.elb.amazonaws.com
- Backend API: http://a2d2c936d192a4057b6cc758b9378e73-1495108477.us-east-1.elb.amazonaws.com/movies

> These temporary AWS lab endpoints may stop working after the lab expires. The screenshots preserve the deployment evidence.
