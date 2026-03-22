# Linkerd (linkerd)
Service mesh without the mess. Linkerd adds security, observability, and reliability to any Kubernetes cluster without the complexity of bloat of other meshes.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/apis.yml)

## Scope

- **Type:** Index 
- **Position:** Consuming 
- **Access:** 3rd-Party 

## Tags:

 - Service Mesh, Kubernetes, Observability, Security, mTLS

## Timestamps

- **Created:** 2025-08-19 
- **Modified:** 2026-03-18 

## APIs

### Linkerd Proxy Admin API
The Linkerd proxy exposes an admin HTTP server on each meshed pod, providing health check endpoints, readiness probes, Prometheus-compatible metrics, and runtime diagnostic information. By default this server listens on port 4191.

**Human URL:** [https://linkerd.io/2-edge/reference/proxy-configuration/](https://linkerd.io/2-edge/reference/proxy-configuration/)


#### Tags:

 - Proxy, Metrics, Health Check, Prometheus

#### Properties

- [Documentation](https://linkerd.io/2-edge/reference/proxy-configuration/)
- [Reference](https://linkerd.io/2-edge/reference/proxy-metrics/)
- [OpenAPI](openapi/linkerd-proxy-admin-openapi.yml)

### Linkerd Viz Metrics API
The Linkerd Viz extension provides a metrics API that powers the linkerd viz CLI commands and the Linkerd dashboard. It queries Prometheus for golden metrics including request volume, success rate, and latency distributions for HTTP, HTTP/2, and gRPC traffic across meshed workloads.

**Human URL:** [https://linkerd.io/2-edge/reference/cli/viz/](https://linkerd.io/2-edge/reference/cli/viz/)


#### Tags:

 - Metrics, Observability, Statistics, Dashboard

#### Properties

- [Documentation](https://linkerd.io/2-edge/reference/cli/viz/)
- [OpenAPI](openapi/linkerd-viz-metrics-openapi.yml)
- [JSONSchema](json-schema/stat-summary.json)
- [JSONSchema](json-schema/edge.json)
- [JSONSchema](json-schema/gateway.json)
- [JSONLD](json-ld/linkerd-context.jsonld)

### Linkerd Tap API
The Linkerd Tap API is a Kubernetes aggregated API server that provides real-time streaming access to requests flowing through the Linkerd service mesh. It allows live inspection of HTTP and gRPC traffic including headers, paths, response codes, and latency. Access is controlled via Kubernetes RBAC.

**Human URL:** [https://linkerd.io/2-edge/reference/cli/viz/](https://linkerd.io/2-edge/reference/cli/viz/)


#### Tags:

 - Tap, Traffic Inspection, Debugging, Real-Time

#### Properties

- [Documentation](https://linkerd.io/2-edge/reference/cli/viz/)
- [OpenAPI](openapi/linkerd-tap-openapi.yml)
- [JSONSchema](json-schema/tap-event.json)
- [JSONLD](json-ld/linkerd-context.jsonld)

### Linkerd Proxy Control Plane API
The Linkerd Proxy Control Plane gRPC API defines the protobuf service contracts used by the data-plane proxy to communicate with the control plane. It includes the Destination API for service discovery and traffic policy, the Identity API for issuing mTLS certificates, and the Inbound API for per-port authorization and rate-limiting policies.

**Human URL:** [https://github.com/linkerd/linkerd2-proxy-api](https://github.com/linkerd/linkerd2-proxy-api)


#### Tags:

 - gRPC, Control Plane, mTLS, Policy

#### Properties

- [Documentation](https://github.com/linkerd/linkerd2-proxy-api)
- [Reference](https://linkerd.io/2-edge/reference/authorization-policy/)
- [GitHubRepository](https://github.com/linkerd/linkerd2-proxy-api)
- [JSONSchema](json-schema/service-profile.json)

### Linkerd Multicluster API
The Linkerd Multicluster extension provides Kubernetes CRDs and a gateway component that enables transparent, secure cross-cluster service communication. It uses mTLS to authenticate workloads across cluster boundaries within a unified trust domain, allowing services in different clusters to communicate as if they were local.

**Human URL:** [https://linkerd.io/2-edge/features/multicluster/](https://linkerd.io/2-edge/features/multicluster/)


#### Tags:

 - Multicluster, Federation, mTLS, Kubernetes

#### Properties

- [Documentation](https://linkerd.io/2-edge/features/multicluster/)
- [Reference](https://linkerd.io/2-edge/reference/multicluster/)

## Common Properties

- [JSON-LD](json-ld/linkerd-context.jsonld)
- [JSONSchema](json-schema/service-profile.json)
- [Website](https://linkerd.io/)
- [Documentation](https://linkerd.io/2.19/reference/)
- [Getting Started](https://linkerd.io/2.19/getting-started/)
- [GitHub Organization](https://github.com/linkerd)
- [GitHubRepository](https://github.com/linkerd/linkerd2)
- [Blog](https://linkerd.io/blog/)
- [Change Log](https://github.com/linkerd/linkerd2/blob/main/CHANGES.md)
- [Community](https://linkerd.io/community/get-involved/)
- [Slack](https://slack.linkerd.io/)
- [Support](https://linkerd.buoyant.io/)
- [Releases](https://github.com/linkerd/linkerd2/releases)
- [Security](https://github.com/linkerd/linkerd2/blob/main/SECURITY.md)
- [Stack Overflow](https://stackoverflow.com/questions/tagged/linkerd)
- [YouTube](https://www.youtube.com/@Linkerd)
- [Privacy Policy](https://buoyant.io/privacy-policy)
- [Terms of Service](https://buoyant.io/terms-of-service)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
