---
title: "Building your Infrastructure with Tilt, Linkerd, and Nginx (part 2)"
url: "https://linkerd.io/2025/07/25/tilt-linkerd-nginx-part-2/"
date: "Fri, 25 Jul 2025 00:00:00 +0000"
author: "Chris Campbell, Linkerd Ambassador"
feed_url: "https://linkerd.io/blog/feed.xml"
---
<p><em>This is part two of a series by Linkerd Ambassador Chris Campbell exploring how
to bridge the gap between development and production by using Linkerd, Tilt, and
Ingress-Nginx to create a robust environment in which you can develop using your
real production infrastructure.</em></p>
<hr />
<p>In <a href="https://linkerd.io/2024/12/02/tilt-linkerd-nginx-part-1/">Part 1</a> of this series, we built a
simple microservices demo with Linkerd on a local Kubernetes cluster using Tilt.
Our demo consists of three services (foo, bar, and baz) that communicate via
HTTP REST. In this second part, we&rsquo;ll extend our demo to support gRPC
communication and explore some of Linkerd&rsquo;s helpful features for managing gRPC
services.</p>
