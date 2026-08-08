# Asad Bashir

DevOps and DevSecOps Engineer based in Islamabad, Pakistan. I build the pipelines
and infrastructure that get code into production safely.

I started as a MERN stack developer and moved into DevOps because the problems I
kept running into were deployment problems, not application problems. I now work
on AWS and Hetzner infrastructure, Kubernetes, CI/CD and secrets management.

[![Portfolio](https://img.shields.io/badge/Portfolio-committodeploy.dev-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://committodeploy.dev)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/asad-bashir-772b73299)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:asadbashir2229526@gmail.com)

## What I do now

DevOps Engineer at CyberoidTech since December 2025. I run production workloads on
ECS Fargate and EKS, provision AWS with Terraform, manage Hetzner dedicated and
cloud servers, and build delivery pipelines with GitHub Actions and ArgoCD using
OIDC authentication so there are no long lived AWS keys anywhere.

On the security side I run HashiCorp Vault with External Secrets Operator, AWS WAF
and least privilege IAM, and I set up AWS Client VPN for secure client access to
private infrastructure. I also responded to CVE-2025-1974 (IngressNightmare) in
production by blocking port 8443 and hardening ingress config across the cluster.

Before this I was a DevOps intern at Techinn360 from June to November 2025,
building GitHub Actions pipelines with OIDC auth and running EC2, RDS, S3,
CloudFront and ALB infrastructure.

## Tech stack

**Cloud**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![ECS Fargate](https://img.shields.io/badge/ECS_Fargate-FF9900?style=flat-square&logo=amazonecs&logoColor=white)
![EKS](https://img.shields.io/badge/EKS-FF9900?style=flat-square&logo=amazoneks&logoColor=white)
![EC2](https://img.shields.io/badge/EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white)
![RDS](https://img.shields.io/badge/RDS-527FFF?style=flat-square&logo=amazonrds&logoColor=white)
![S3](https://img.shields.io/badge/S3-569A31?style=flat-square&logo=amazons3&logoColor=white)
![CloudFront](https://img.shields.io/badge/CloudFront-8C4FFF?style=flat-square&logo=amazonwebservices&logoColor=white)
![Client VPN](https://img.shields.io/badge/Client_VPN-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Hetzner](https://img.shields.io/badge/Hetzner-D50C2D?style=flat-square&logo=hetzner&logoColor=white)

**Infrastructure as code and config**

![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**Containers and orchestration**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)

**CI/CD and security**

![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Vault](https://img.shields.io/badge/Vault-FFEC6E?style=flat-square&logo=vault&logoColor=black)
![OIDC](https://img.shields.io/badge/OIDC-000000?style=flat-square&logo=openid&logoColor=white)
![Snyk](https://img.shields.io/badge/Snyk-4C4A73?style=flat-square&logo=snyk&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=flat-square&logo=aquasecurity&logoColor=white)

**Monitoring**

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Loki](https://img.shields.io/badge/Loki-F5A800?style=flat-square&logo=grafana&logoColor=white)

**Databases and application**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)

## Projects

### Infrastructure and CI/CD

**[shopix-aws-production](https://github.com/asadbashir7755/shopix-aws-production)**
A full stack ecommerce platform on a custom AWS VPC. ALB across two availability
zones, app servers in private subnets, RDS MySQL with no public exposure, NAT
Gateway for outbound traffic. Deploys through GitHub Actions using OIDC, so there
are no static AWS keys, and server access goes through SSM instead of SSH.

**[wanderlust-jenkins-cicd](https://github.com/asadbashir7755/wanderlust-jenkins-cicd)**
A Jenkins pipeline on a self hosted agent. Tests, builds both images in parallel,
pushes to a registry and deploys with Compose, with health checks, smoke tests and
a rollback script. All secrets come from the Jenkins credential store.

**[jenkins-shared-library](https://github.com/asadbashir7755/jenkins-shared-library)**
The Groovy shared library behind that pipeline: clone, backend_test, docker_build,
docker_push and envconfig.

**[fyp-github-actions-cicd](https://github.com/asadbashir7755/fyp-github-actions-cicd)**
GitHub Actions CI for a three tier React, Express and PostgreSQL app, with per
workspace dependency caching and a production build check.

### Platform

**[kubernetes-projects](https://github.com/asadbashir7755/kubernetes-projects)**
Deployments, StatefulSets, Services, probes, autoscaling, volumes and ingress
routing, all applied to real clusters.

**[docker-projects](https://github.com/asadbashir7755/docker-projects)**
Builds up from a single Dockerfile to a three tier stack behind Nginx.

**[terraform-learning](https://github.com/asadbashir7755/terraform-learning)**,
**[ansible-learning](https://github.com/asadbashir7755/ansible-learning)**,
**[linux-administration](https://github.com/asadbashir7755/linux-administration)**
Infrastructure as code, config management including a role based LAMP deployment
with encrypted per environment secrets, and 18 sessions of Linux administration.

### Before DevOps

**[furnished-home-rental](https://github.com/asadbashir7755/furnished-home-rental)**
MERN rental platform with search, availability, Stripe payments and an admin
dashboard. Final year project.

**[web-dev-practice](https://github.com/asadbashir7755/web-dev-practice)**
The web development work that led into all of this.

**[cpp-foundations](https://github.com/asadbashir7755/cpp-foundations)**
C++ teaching material written while mentoring a junior developer.

## Certifications

AWS Certified Cloud Practitioner, Amazon Web Services

Ansible Automation, Udemy School of DevOps

AWS Solutions Architect Associate, in progress

## Education

BS Computer Science, 2021 to 2025
