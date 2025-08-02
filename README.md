# project11-irsa-s3-access
Project 11: Secure access to S3 from an EKS Pod using IAM Roles for Service Accounts (IRSA). Demonstrates least-privilege access control using service account trust and AWS CLI.
 Project 11: Securing Kubernetes Workloads on AWS EKS
Project 11: Securing Kubernetes Workloads on AWS EKS
Title:
Enterprise Kubernetes Security Hardening: Implementing Fine-Grained Access Controls & Observability on AWS EKS
Project Overview
This project simulates a real-world enterprise use case where containerized workloads in Amazon EKS must be secured using best practices. It focuses on implementing fine-grained access controls, pod identity isolation, network segmentation, and comprehensive observability.
Aim
To demonstrate and implement Kubernetes-native security features—such as RBAC, Network Policies, and IAM Roles for Service Accounts (IRSA)—in an Amazon EKS cluster while maintaining full visibility through CloudWatch and CloudTrail.
Project Objectives
- Provision a secure EKS cluster using eksctl and AWS CLI.
- Enable IAM Roles for Service Accounts (IRSA) for least-privilege pod access.
- Implement Kubernetes RBAC to enforce least-privilege user permissions.
- Deploy a sample application with Network Policies to control pod communication.
- Enable CloudWatch and CloudTrail for observability and audit logging.
- Enforce Pod Security Standards (PSS) at the restricted or baseline level.
- Document the project in detail for public portfolio and recruiter visibility.
Tools, Platforms & Services
| Tool / Service | Purpose |
|----------------|---------|
| AWS EKS | Kubernetes orchestration |
| eksctl | EKS provisioning |
| kubectl | Kubernetes CLI |
| IAM + IRSA | Pod-level IAM policies |
| VPC & Subnets | Cluster network isolation |
| Calico / Cilium | Kubernetes Network Policies |
| AWS CloudWatch | Observability |
| AWS CloudTrail | Audit logging |
| VS Code | Local development |
| GitHub | Documentation |
Why This Project Matters to Employers
- Security-Centric Kubernetes Operations
- Production-Ready Architecture
- Cost-Efficient Observability
- Compliance & Zero Trust
- Modern DevSecOps Practices
Methodology & Procedure
Step-by-step execution with screenshots was taken at each major stage.
Steps:
1. Environment Setup: Installed AWS CLI, eksctl, kubectl.
2. EKS Cluster Creation via eksctl with IRSA enabled.
3. IAM Roles for Service Accounts (IRSA) created and tested with a sample pod.
4. Kubernetes RBAC Role and RoleBinding deployed.
5. Network Policies enforced via Calico/Cilium.
6. CloudWatch and CloudTrail enabled for observability.
7. Pod Security Standards applied using PodSecurity labels.
Screenshots
All terminal output, YAML files, IAM roles, CloudWatch logs, and Kubernetes manifests are documented with 33+ screenshots for full reproducibility.
Skills Demonstrated
- Kubernetes IAM (IRSA)
- Infrastructure-as-Code (eksctl)
- RBAC, Pod Identity, Network Policies
- AWS CloudWatch/CloudTrail observability
- GitHub documentation
Challenges & Resolutions
| Challenge | Resolution |
|----------|------------|
| Pod failed to assume IAM Role | Fixed trust relationship |
| S3 access denied | Verified CloudTrail logs |
| NetworkPolicy didn't block traffic | Calico validation done |
Future Improvements
- Add OPA/Gatekeeper
- Integrate GuardDuty
- Use AWS Secrets Manager
License: MIT
🤝 Connect:
- LinkedIn: https://www.linkedin.com/in/ime-ben-8aa008362
- GitHub: https://github.com/ime-cloud-sec-analyst
Author Information –Ime Ben
•	Full Name: Dr. Ime Ben
•	GitHub: ime-cloud-sec-analyst
•	LinkedIn: linkedin.com/in/ime-ben-8aa008362
•	Email: imegcu55@gmail.com
•	Role: AWS Cloud Security & DevSecOps Engineer
•	Certifications: AWS Security Speciality, Terraform Associate, Azure Security Engineer
•	Location: Glasgow, Scotland (Available for Remote/Contract Roles)
•	Portfolio: 30+ Security Projects on GitHub | Hands-on Labs | SIEM | SOAR | IAM | Terraform | EKS | GuardDuty
