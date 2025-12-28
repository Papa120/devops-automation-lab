# CI/CD Pipeline for Kubernetes

This project demonstrates a production-style CI/CD pipeline that:
	•	Builds Docker images
	•	Pushes images to a container registry
	•	Deploys applications to Kubernetes using rolling updates
	•	Supports fast rollback on deployment failure
## Tech Stack
	•	Jenkins (Declarative Pipeline)
	•	Docker
	•	Kubernetes
	•	Python (Flask)

## Pipeline Flow
	1.	Code pushed to the repository
	2.	Jenkins checks out the source code
	3.	Jenkins builds and tags the Docker image
	4.	Image is pushed to the container registry
	5.	Kubernetes deployment is updated
	6.	Rollout status is monitored, and rollback is available

## How to Run
```bash
kubectl apply -f manifests/
