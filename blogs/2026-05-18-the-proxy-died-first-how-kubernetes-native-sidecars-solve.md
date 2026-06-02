---
title: "The Proxy Died First: How Kubernetes Native Sidecars Solve the Service Mesh Shutdown Problem"
url: "https://linkerd.io/2026/05/18/the-proxy-died-first/"
date: "2026-05-18"
author: "Blake Romano, Linkerd Ambassador"
feed_url: "https://linkerd.io/blog/feed.xml"
---
If you’ve ever operated a service mesh on Kubernetes, you’ve probably seen something like this during a rolling deployment: Unexpected error occurred: Client 'http://my-api:8080/': Connect Error: Connection refused: my-api/100.20.100.200:8080 One second your pod is humming along, serving traffic, and talking to its upstream dependencies through the mesh. The next second it enters Terminating state, the sidecar proxy exits, and every in-flight request to a dependent service gets a cold Connection refused in response.
