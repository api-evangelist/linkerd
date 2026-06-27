---
title: "Federating Clusters for Zero-Downtime Kubernetes"
url: "https://linkerd.io/2026/06/24/federating-clusters-for-zero-downtime-kubernetes/"
date: "2026-06-24"
author: "Dominik Táskai, Linkerd Ambassador"
feed_url: "https://linkerd.io/blog/feed.xml"
---
Every multi-region setup eventually meets the same awkward moment: a whole cluster goes away, and the identical copy of your service running two regions over might as well not exist, because nothing is wired to treat them as one thing. Failover becomes a runbook: restore, repoint DNS, and wait for an outage that, on paper, you’d already paid to survive. Linkerd’s multicluster extension closes that gap by letting several clusters present a service as a single, load-balanced endpoint.
