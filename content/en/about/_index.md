---
title: About
menu:
  main:
    weight: 10
cascade:
- type: "_default"
---

<!--add blocks of content here to add more sections to the community page -->

{{< blocks/cover title="About Kuberenets Cluster API ..." image_anchor="top" >}}
<div class="mx-auto">
	<p class="lead mt-5">The Who, the Why.</p>
	{{< blocks/link-down color="info" >}}
</div>
{{< /blocks/cover >}}

{{% blocks/lead color="primary" %}}
Cluster API is a Kubernetes sub-project focused on providing declarative APIs and tooling to simplify provisioning, upgrading, and operating multiple Kubernetes clusters.

{{% /blocks/lead %}}


{{% blocks/section %}}

Started by the Kubernetes Special Interest Group (SIG) [Cluster Lifecycle](https://github.com/kubernetes/community/tree/master/sig-cluster-lifecycle#readme), the Cluster API project uses Kubernetes-style APIs and patterns to automate cluster lifecycle management for platform operators. The supporting infrastructure, like virtual machines, networks, load balancers, and VPCs, as well as the Kubernetes cluster configuration are all defined in the same way that application developers operate deploying and managing their workloads. This enables consistent and repeatable cluster deployments across a wide variety of infrastructure environments.
{{% /blocks/section %}}