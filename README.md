# envoy-k8s-proxy

This repository is fully experimental. It's main goal is to create an envoy-kubernetes setup which will contain an envoy pod as an ingress kubernetes cluster gateway, and a worker pod with two additional containers. Worker pod will consist an RTP engine container and a sidecar envoy container.

Final setup will look something like this: User A -> envoy-ingressGW -> worker(envoy sidecar) -> worker(RTP engine) -> worker(envoy sidecar) -> envoy-ingressGW -> User B and vice versa.

