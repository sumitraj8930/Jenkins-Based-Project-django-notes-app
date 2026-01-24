
# **CI/CD Pipeline with Jenkins Shared Libraries & AWS EKS Deployment**

A fully automated CI/CD pipeline that leverages **Jenkins Shared Libraries**, **Docker**, and **AWS EKS** to standardize software delivery workflows, containerize applications, and deploy reliably into a Kubernetes environment with observability and monitoring enabled.

---

## **Project Overview**

This project focuses on implementing scalable DevOps practices through pipeline automation, reusable shared functions, and cloud-native deployment strategies. The solution reduces manual effort, increases deployment consistency, and enables real-time cluster monitoring for performance validation.

---

## **Core Objectives**

* Standardize CI/CD workflows using Shared Libraries
* Enable consistent build and deployment automation
* Deploy containerized workloads to AWS EKS
* Integrate observability for performance insights
* Improve operational efficiency and scalability

---

## **Key Features**

* CI/CD pipeline triggered via GitHub webhook
* Docker image build & registry push automation
* Kubernetes deployment to AWS EKS
* AWS ALB ingress for application exposure
* Shared Libraries for modular pipeline logic
* Monitoring with Prometheus & Grafana
* Secure credential and Docker registry integration

---

## **Architecture Workflow**

```text
GitHub → Jenkins → Docker Build → Docker Push → EKS Deploy → Verify → Monitor
```

---

## **Technology Stack**

**CI/CD:** Jenkins, Shared Libraries, GitHub Webhooks
**Containers:** Docker
**Orchestration:** Kubernetes (Deployments, Services, Ingress, Rolling Updates)
**Cloud:** AWS (EKS, EC2, IAM, VPC, CloudWatch, ALB)
**Monitoring:** Prometheus, Grafana
**Registry:** DockerHub
**Scripting:** Shell/Bash

---

## **Pipeline Stages**

1. Source Code Checkout
2. Build & Test
3. Docker Image Build
4. Docker Registry Push
5. Kubernetes Deployment to EKS
6. Post-Deployment Validation
7. Observability & Monitoring

---

## **Role in DevOps Lifecycle**

✔ Enhances deployment reliability
✔ Reduces manual intervention
✔ Improves pipeline consistency through shared code
✔ Enables cloud-native delivery practices
✔ Supports iterative releases

---

## **Troubleshooting & Debugging**

* Debugged CI failures and deployment issues
* Performed root cause analysis for image build errors
* Validated Kubernetes workloads post deployment
* Fixed pipeline configuration inconsistencies across stages

---

## **Impact & Outcomes**

* Reduced repetitive pipeline logic via Shared Libraries
* Improved scalability for multi-service deployments
* Achieved consistent build-to-deploy transitions
* Enabled visibility into cluster performance metrics
* Strengthened release automation & DevOps workflows

---


