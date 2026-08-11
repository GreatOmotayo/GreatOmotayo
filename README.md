# Hi, I'm Omotayo Ogunrinde 👋

### Cloud Engineer | Azure | Terraform | CI/CD | Cloud Infrastructure | Platform Engineering

I'm a software engineer with 8+ years of experience building backend and full-stack applications, now specializing in **cloud infrastructure and platform engineering**.

I build hands-on Azure environments that go beyond provisioning resources. My projects focus on **governance, security, automation, reliability, observability, and cost control**, with infrastructure defined as code and validated through real tests.

I document the architecture, engineering decisions, trade-offs, failures, troubleshooting, and production limitations behind each build.

---

## ☁️ Cloud Engineering Portfolio

### 🏗️ Multi-Subscription Azure Landing Zone

**Azure Management Groups · Azure Policy · RBAC · Entra ID · Terraform · GitHub Actions · OIDC · Cost Governance**

A Terraform-managed Azure Landing Zone spanning **three subscriptions under one Entra ID tenant**: Platform, Production, and NonProd.

The environment implements:

* Management Group hierarchy
* Policy-as-code guardrails
* Custom RBAC roles
* Entra ID security groups managed as code
* Subscription-level budgets and alerts
* OIDC-authenticated GitHub Actions
* Human approval before production changes
* Differentiated Production and NonProd governance

The project also validates the controls through deliberate enforcement tests rather than assuming that a deployed policy works.

**→ [View the Landing Zone repository](https://github.com/GreatOmotayo/azure-multi-subscription-landing-zone)**

---

### 💰 Automated Azure Cost Governance & Waste Detection

**Azure Policy · Azure Resource Graph · Azure Functions · Cost Management · Managed Identity · Terraform · FinOps**

An automated cost-governance system designed around two complementary controls:

**Prevent:** enforce cost-accountability tags and monitor subscription budgets.

**Detect:** automatically identify waste that still gets through, including unattached managed disks, unassociated public IPs, and stopped-but-not-deallocated virtual machines.

The waste scanner queries Azure Resource Graph, prices findings using Azure's Retail Prices API, and produces recurring reports combining waste findings with Azure Cost Management data.

The project deliberately seeds waste resources so the detection system can be tested against known conditions.

**→ [View the FinOps repository](https://github.com/GreatOmotayo/azure-cost-governance-and-waste-detection)**

---

### ⚙️ Terraform + GitHub Actions CI/CD Pipeline

**Terraform · GitHub Actions · OIDC · Docker · Azure Container Registry · App Service · Managed Identity**

An end-to-end deployment pipeline that provisions Azure infrastructure, builds a container image, pushes it to a private Azure Container Registry, and deploys it to Azure App Service.

The pipeline includes:

* Terraform plan on pull requests
* Plan output posted directly to the PR
* Human review before production changes
* Terraform apply after merge
* Docker image builds tagged with Git commit SHA
* Private ACR with admin credentials disabled
* Managed Identity for App Service → ACR authentication
* OIDC for GitHub Actions → Azure authentication
* Remote Terraform state
* Manual rollback using a previously built image

The project deliberately uses App Service rather than AKS so the focus remains on **CI/CD, Infrastructure as Code, identity, security, and deployment mechanics**.

**→ [View the CI/CD repository](https://github.com/GreatOmotayo/azure-terraform-cicd-pipeline)**

---

## 🧠 How I Build

I try to treat portfolio infrastructure like real engineering work rather than a collection of tutorials.

Each major project focuses on:

**Architecture**

Why the environment is structured the way it is.

**Infrastructure as Code**

Terraform-managed infrastructure that can be reproduced and reviewed.

**Security**

Least privilege, managed identities, OIDC, RBAC and controlled access.

**Governance**

Policies, guardrails, budgets and environment-specific controls.

**Testing**

Deliberately testing controls and documenting expected versus actual behavior.

**Troubleshooting**

Keeping a record of real failures, root causes and fixes.

**Engineering Decisions**

Documenting alternatives, trade-offs and why a particular approach was chosen.

**Production Thinking**

Clearly identifying what is appropriate for a lab and what I would change for a production environment.

---

## 🎯 Engineering Focus

* Azure Cloud Infrastructure
* Cloud Governance
* Infrastructure as Code
* Terraform
* Azure Policy
* RBAC and Identity
* Zero-Trust Architecture
* CI/CD Automation
* Cloud Security
* FinOps and Cost Optimization
* Observability and Reliability
* Container Platforms
* Platform Engineering

---

## 🛠️ Technology

### Cloud

Azure · AWS · GCP

### Infrastructure as Code

Terraform · Bicep

### CI/CD

GitHub Actions · Azure DevOps

### Azure

Azure Management Groups · Azure Policy · RBAC · Entra ID · VNets · Azure Firewall · Azure Bastion · Private Endpoints · Private DNS · Key Vault · Azure Monitor · Log Analytics · Azure Resource Graph · Cost Management

### Containers

Docker · Kubernetes · AKS · Helm

### Development

Node.js · TypeScript · PHP · Laravel · Python · SQL

---

## 🚧 Currently Building

I'm continuing to expand the portfolio from individual infrastructure capabilities toward a complete Azure platform.

Upcoming work includes:

* 🔐 Hub-and-Spoke Network Architecture with Zero-Trust Access
* 📊 Full Azure Observability and Incident Response
* 🚀 Highly Available and Auto-Scaling Application Platform
* ☸️ AKS / Kubernetes Platform Engineering
* 🛡️ Automated Cloud Security and Compliance
* 🌍 Disaster Recovery and Multi-Region Architecture

---

## 📚 Engineering Philosophy

> **Infrastructure that works once is a demo. Infrastructure that can be reproduced, tested, secured, monitored, and explained is engineering.**

I'm documenting the journey publicly through GitHub and LinkedIn, including the decisions that worked, the decisions that didn't, and what I would change if I were building each environment for production.

---

## 🔗 Connect

**LinkedIn:** [Connect with me](YOUR_LINKEDIN_URL)

**GitHub:** [GreatOmotayo](https://github.com/GreatOmotayo)
