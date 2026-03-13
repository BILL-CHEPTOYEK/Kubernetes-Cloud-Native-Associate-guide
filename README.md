<div align="center">
  <img src="https://raw.githubusercontent.com/cncf/artwork/master/other/kcna/icon/color/kcna-icon-color.png" width="150" alt="KCNA Logo">
  
  # Kubernetes and Cloud Native Associate (KCNA) Certification Guide
  
  **A comprehensive, open-source guide and study repository for the KCNA certification.**
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
  [![Cloud Native Computing Foundation](https://img.shields.io/badge/CNCF-Certification-blue?style=flat-square)](https://training.linuxfoundation.org/certification/kubernetes-cloud-native-associate/)
  
  [Overview](#-certification-overview) • [Curriculum](#-exam-domains) • [Study Guide & Path](#-study-guide--path) • [Labs](#-hands-on-labs) • [Resources](#-resources)
</div>

---

## Certification Overview
The **Kubernetes and Cloud Native Associate (KCNA)** exam by the CNCF tests a user’s foundational knowledge and skills in Kubernetes and the wider cloud-native ecosystem. 

Unlike the performance-based CKA/CKAD, **KCNA is multiple-choice**, testing your conceptual understanding of modern cloud-native architectures, container orchestration, GitOps, observability, and CNCF projects.

* **Format:** 60 Multiple-choice questions
* **Duration:** 90 minutes
* **Cost:** ~$250 USD
* **Passing Score:** 75%
* **Validity:** 3 Years
* **Prerequisites:** None (though basic Linux/IT concepts are very helpful)

---

## Exam Domains

The exam curriculum is distributed across five main areas. This repository strictly maps directly to these domains so you can effectively track your study coverage.

| Domain | Weight | Core Topics Covered |
|--------|--------|-------------|
| **1. Kubernetes Fundamentals** | **46%** | Architecture, API, Scheduling, Resources (Pods, Deployments, ReplicaSets) |
| **2. Container Orchestration** | **22%** | Container Runtimes (containerd), Security, Networking, Service Mesh |
| **3. Cloud Native Architecture** | **16%** | Serverless, Autoscaling, Open Standards, Open Source Governance, Personas |
| **4. Application Delivery** | **8%** | CI/CD processes, GitOps, Application Deployment Strategies |
| **5. Observability** | **8%** | Logging, Metrics, Tracing, Prometheus, Cost Management |

---

## Study Guide & Path

Whether you have 2 weeks or 2 months, pacing is critical. You can see our recommended **[Weekly Study Plan](study-plan/study-plan.md)**, but we suggest following this sequential path for the most intuitive learning experience:

### Phase 1: Theory (LFS250 Breakdowns)
Read through the localized concept summaries. These cover the fundamental knowledge map for the *CNCF Kubernetes and Cloud Native Essentials (LFS250)* track.
1. [01. Cloud Native Intro](lfs250-summary/01-cloud-native-intro.md)
2. [02. Containers Deep Dive](lfs250-summary/02-containers.md)
3. [03. Kubernetes Architecture](lfs250-summary/03-kubernetes-architecture.md)
4. [04. Kubernetes Objects](lfs250-summary/04-kubernetes-objects.md)
5. [05. Networking & Ingress](lfs250-summary/05-networking.md)
6. [06. Observability (Logs, Metrics, Traces)](lfs250-summary/06-observability.md)
7. [07. Application Delivery (CI/CD & GitOps)](lfs250-summary/07-application-delivery.md)
8. [08. The CNCF Ecosystem](lfs250-summary/08-cncf-ecosystem.md)

### 💻 Phase 2: Hands-on Labs
Even though KCNA is entirely multiple choice, deploying clusters locally significantly reinforces the theory.
* [1. Setup Minikube Locally](labs/minikube-setup.md)
* [2. Deploying Your First Pod](labs/first-pod.md)
* [3. Deployments & Rollouts](labs/deployments.md)
* [4. Exposing Traffic with Services](labs/services.md)
* [5. Scaling Applications](labs/scaling.md)

### Phase 3: Practice & Mock Exams
Test what you have learned before attempting the real exam.
* **Topic Checks:** 
  * [KCNA Fundamentals](practice-questions/kcna-fundamentals.md)
  * [Cloud Native Concepts](practice-questions/cloud-native.md) 
  * [Observability](practice-questions/observability.md)
* **Full Mocks:** 
  * [Mock Exam 1](practice-questions/mock-exams/mock-exam-1.md)
  * [Mock Exam 2](practice-questions/mock-exams/mock-exam-2.md)
  * [Mock Exam 3](practice-questions/mock-exams/mock-exam-3.md)

### Phase 4: Final Polish (Cheat Sheets)
Review these strictly the week of your exam.
* [Kubernetes Architecture Diagram & Notes](cheat-sheets/kubernetes-architecture-cheatsheet.md)
* [Essential Kubectl Commands](cheat-sheets/kubectl-cheatsheet.md)
* **[The Ultimate Last-Minute KCNA Review](cheat-sheets/kcna-last-minute-review.md)**

---

## The CNCF Cloud Native Landscape (Cheat Sheet)
You don't need to know how to install or configure all of these tools, but you *must* know what category they belong to and their basic use-case concept for the exam:
* **Container Runtimes:** `containerd`, `CRI-O`, `Docker`
* **Service Mesh:** `Envoy`, `Linkerd`, `Istio`
* **Networking (CNI):** `Cilium`, `Calico`, `Flannel`, `CoreDNS`
* **Observability:** `Prometheus` (Metrics), `Fluentd` (Logging), `Jaeger` (Tracing), `OpenTelemetry`
* **App Delivery (GitOps):** `Helm`, `ArgoCD`, `Flux`
* **Security:** `OPA` (Open Policy Agent for Policies), `Falco` (Runtime Security), `Trivy` (Scanning)

---

## Resources
Looking for more official documentation, video courses, and deeper open-source references?  
👉 **[View our curated resources list](resources/resources.md)**

---

## Contributing
Found a typo, have a new practice question idea, or want to add a better diagram? This repository is open-source and contributions are extremely welcome!

1. Fork the Project
2. Create your Feature Branch: `git checkout -b feature/cool-addition`
3. Commit your Changes: `git commit -m 'Add some feature'`
4. Push to the Branch: `git push origin feature/cool-addition`
5. Open a Pull Request

---

<p align="center"><i>Good luck on your KCNA journey! You've got this!</i></p>