# Linkerd (linkerd)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Service mesh without the mess. Linkerd adds security, observability, and reliability to any Kubernetes cluster without the complexity of bloat of other meshes.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/linkerd/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Kubernetes
- mTLS
- Observability
- Security
- Service Mesh

## Timestamps

- **Created:** 2025-08-19
- **Modified:** 2026-05-19

## APIs

### Linkerd Proxy Admin API

The Linkerd proxy exposes an admin HTTP server on each meshed pod, providing health check endpoints, readiness probes, Prometheus-compatible metrics, and runtime diagnostic information. By default this server listens on port 4191.

- **Human URL:** [https://linkerd.io/2-edge/reference/proxy-configuration/](https://linkerd.io/2-edge/reference/proxy-configuration/)
- **Base URL:** `http://localhost:4191`

#### Tags

- Health Check
- Metrics
- Prometheus
- Proxy

#### Properties

- [Documentation](https://linkerd.io/2-edge/reference/proxy-configuration/)
- [Reference](https://linkerd.io/2-edge/reference/proxy-metrics/)
- [OpenAPI](openapi/linkerd-proxy-admin-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/linkerd-proxy-admin.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-proxy-admin.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linkerd Viz Metrics API

The Linkerd Viz extension provides a metrics API that powers the linkerd viz CLI commands and the Linkerd dashboard. It queries Prometheus for golden metrics including request volume, success rate, and latency distributions for HTTP, HTTP/2, and gRPC traffic across meshed workloads.

- **Human URL:** [https://linkerd.io/2-edge/reference/cli/viz/](https://linkerd.io/2-edge/reference/cli/viz/)

#### Tags

- Dashboard
- Metrics
- Observability
- Statistics

#### Properties

- [Documentation](https://linkerd.io/2-edge/reference/cli/viz/)
- [OpenAPI](openapi/linkerd-viz-metrics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/linkerd-viz-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-viz-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/stat-summary.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/edge.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/gateway.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/linkerd-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Linkerd Tap API

The Linkerd Tap API is a Kubernetes aggregated API server that provides real-time streaming access to requests flowing through the Linkerd service mesh. It allows live inspection of HTTP and gRPC traffic including headers, paths, response codes, and latency. Access is controlled via Kubernetes RBAC.

- **Human URL:** [https://linkerd.io/2-edge/reference/cli/viz/](https://linkerd.io/2-edge/reference/cli/viz/)

#### Tags

- Debugging
- Real-Time
- Tap
- Traffic Inspection

#### Properties

- [Documentation](https://linkerd.io/2-edge/reference/cli/viz/)
- [OpenAPI](openapi/linkerd-tap-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/linkerd-tap.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-tap.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/tap-event.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/linkerd-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Linkerd Proxy Control Plane API

The Linkerd Proxy Control Plane gRPC API defines the protobuf service contracts used by the data-plane proxy to communicate with the control plane. It includes the Destination API for service discovery and traffic policy, the Identity API for issuing mTLS certificates, and the Inbound API for per-port authorization and rate-limiting policies.

- **Human URL:** [https://github.com/linkerd/linkerd2-proxy-api](https://github.com/linkerd/linkerd2-proxy-api)

#### Tags

- Control Plane
- gRPC
- mTLS
- Policy

#### Properties

- [Documentation](https://github.com/linkerd/linkerd2-proxy-api)
- [Reference](https://linkerd.io/2-edge/reference/authorization-policy/)
- [GitHub Repository](https://github.com/linkerd/linkerd2-proxy-api)
- [JSON Schema](json-schema/service-profile.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/linkerd-proxy-admin.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-proxy-admin.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/linkerd-tap.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-tap.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/linkerd-viz-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-viz-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Linkerd Multicluster API

The Linkerd Multicluster extension provides Kubernetes CRDs and a gateway component that enables transparent, secure cross-cluster service communication. It uses mTLS to authenticate workloads across cluster boundaries within a unified trust domain, allowing services in different clusters to communicate as if they were local.

- **Human URL:** [https://linkerd.io/2-edge/features/multicluster/](https://linkerd.io/2-edge/features/multicluster/)

#### Tags

- Federation
- Kubernetes
- mTLS
- Multicluster

#### Properties

- [Documentation](https://linkerd.io/2-edge/features/multicluster/)
- [Reference](https://linkerd.io/2-edge/reference/multicluster/)
- [Postman Collection](collections/linkerd-proxy-admin.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-proxy-admin.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/linkerd-tap.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-tap.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/linkerd-viz-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/linkerd-viz-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/linkerd)
- [JSON-LD](json-ld/linkerd-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/service-profile.json) — [JSON Schema](https://json-schema.org/specification)
- [Website](https://linkerd.io/)
- [Documentation](https://linkerd.io/2.19/reference/)
- [Getting Started](https://linkerd.io/2.19/getting-started/)
- [GitHub Organization](https://github.com/linkerd)
- [GitHub Repository](https://github.com/linkerd/linkerd2)
- [Blog](https://linkerd.io/blog/)
- [Changelog](https://github.com/linkerd/linkerd2/blob/main/CHANGES.md)
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
