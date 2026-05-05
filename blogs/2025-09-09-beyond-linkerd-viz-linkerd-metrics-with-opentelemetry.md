---
title: "Beyond linkerd-viz: Linkerd Metrics with OpenTelemetry"
url: "https://linkerd.io/2025/09/09/linkerd-with-opentelemetry/"
date: "Tue, 09 Sep 2025 00:00:00 +0000"
author: "Eli Goldberg, Linkerd Ambassador"
feed_url: "https://linkerd.io/blog/feed.xml"
---
<h2 id="tldr">TL;DR</h2>
<p>Linkerd, the enterprise-grade service mesh that minimizes overhead, now
integrates with <a href="https://opentelemetry.io/" rel="noopener" target="_blank">OpenTelemetry</a>, often also simply
called OTel. That&rsquo;s pretty cool because it allows you to collect and export
Linkerd&rsquo;s metrics to your favorite observability tools. This integration
improves your ability to monitor and troubleshoot applications effectively.
Sounds interesting? Read on.</p>
<p>Before we dive into this topic, I want to be sure you have a basic understanding
of Kubernetes. If you&rsquo;re new to it, that&rsquo;s ok! But I&rsquo;d recommend exploring the
official Kubernetes tutorials and/or experimenting with &ldquo;Kind&rdquo; (Kubernetes in
Docker) with
<a href="https://kind.sigs.k8s.io/docs/user/quick-start/" rel="noopener" target="_blank">this simple guide</a>.</p>
