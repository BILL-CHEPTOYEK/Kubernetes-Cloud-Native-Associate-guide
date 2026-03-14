# Cloud Native Observability

## Introduction

### Learning Objectives

By the end of this chapter, you should be able to:

- Explain why observability is a key discipline of cloud computing
- Discuss metrics, logs, and traces
- Understand how to show logs of containerized applications
- Explain how Prometheus can be used to collect and store metrics
- Understand how to optimize cloud costs

## Observability

Observability is broader than monitoring. Originating in control theory, observability focuses on understanding a system's internal state from its external outputs. In cloud native systems this helps teams answer questions about stability, sensitivity to conditions, thresholds, failures, and bottlenecks.

## Telemetry

Telemetry is the collection and transmission of measurements. In cloud native systems telemetry typically falls into three categories:

- Logs: messages emitted by applications recording events, errors, or debugging information.
- Metrics: quantitative measurements over time (request rates, CPU/memory, error rates).
- Traces: records tracking a request's lifecycle across distributed services, showing timing and where time is spent.

Centralized telemetry is essential in distributed systems; storing logs locally is impractical at scale.

## Logs (how to show container logs)

To view logs for a container in Kubernetes:

```bash
kubectl logs <pod-name> [-c <container-name>]
```

For streaming logs:

```bash
kubectl logs -f <pod-name>
```

In production you typically forward logs to a centralized system (e.g., Elasticsearch, Loki, or a cloud logging service).

## Metrics and Prometheus

Prometheus collects metrics by scraping HTTP endpoints that expose metrics in a specific format (Prometheus exposition format). Key points:

- Targets expose metrics (often at `/metrics`)
- Prometheus server scrapes targets at configured intervals
- Metrics are stored as time-series and queried with PromQL

Prometheus works well with exporters that translate system metrics into Prometheus format (node_exporter, kube-state-metrics).

## Tracing

Tracing captures the end-to-end path of a request through services. Tools like Jaeger and Zipkin collect spans and visualize traces to help find latency hotspots and errors across microservices.

## OpenTelemetry

OpenTelemetry provides vendor-neutral APIs and SDKs to instrument applications for logs, metrics, and traces, simplifying integration with backends like Prometheus, Jaeger, and cloud services.

## Cost Management

Optimizing cloud costs requires telemetry-driven decisions: right-sizing resources, autoscaling, using spot/preemptible instances, and shutting down unused environments. Tools like OpenCost can help attribute costs to Kubernetes workloads.

## Additional Resources

- Prometheus docs, OpenTelemetry, Jaeger, Loki, OpenCost

## Knowledge Check

- Chapter 7 Quiz