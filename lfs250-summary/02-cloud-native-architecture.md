# Cloud Native Architecture

## Introduction

### Learning Objectives

By the end of this chapter, you should be able to:

- Explain the goals of cloud native architecture (cost efficiency, reliability, faster time-to-market)
- Describe common cloud native building blocks (containers, microservices, immutable infrastructure)
- Compare monolithic and microservice architectures and trade-offs
- Describe autoscaling patterns and when to use them

## Understanding the Cloud Native Architecture

At its core, cloud native architecture optimizes software for cost efficiency, reliability, and faster time-to-market by combining cultural, technological, and architectural design patterns.

The Cloud Native Computing Foundation defines cloud native practices as those that empower organizations to develop, build, and deploy workloads in computing environments at scale in a programmatic and repeatable manner. Cloud native systems are loosely coupled, secure, resilient, manageable, sustainable, and observable.

Cloud native technologies typically include containers, service meshes, multi-tenancy, microservices, immutable infrastructure, serverless, and declarative APIs.

## Monolithic vs Microservices

Traditional monolithic apps are self-contained; cloud native architecture breaks applications into smaller services (microservices) that can be developed, scaled, and deployed independently.

## Characteristics of Cloud Native Architecture

- High automation (CI/CD, infrastructure-as-code)
- Self-healing (health checks, restarts)
- Scalable (horizontal and vertical scaling)
- Cost efficient (scale to zero, usage-based pricing)
- Easy to maintain (smaller services, independent teams)
- Secure by default (zero-trust patterns)

## Autoscaling

Autoscaling dynamically adjusts resources in response to demand. Horizontal scaling adds instances; vertical scaling increases resources for an instance. Cloud platforms make horizontal autoscaling fast and cost-effective; configure min/max instances and metrics that trigger scaling.

## Additional Resources

- Twelve-Factor App
- CNCF projects and guidelines