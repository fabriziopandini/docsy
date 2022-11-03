---
title: "CRDs"
weight: 20
description: |
  Documentation about Cluster API Custom Resource Definitions.
---

[CRDs](https://doc.crds.dev/github.com/kubernetes-sigs/cluster-api)

## Relationships

There are many resources that appear in the Cluster API. In this section, we use diagrams to illustrate the most common relationships between Cluster API resources.

{{< alert >}}

The straight lines represent "management". For example, "MachineSet manages Machines". The dotted line represents "reference". For example, "Machine's `spec.infrastructureRef` field references FooMachine".

The direction of the arrows indicates the direction of "management" or "reference". For example, "the relationship between MachineSet and Machine is management from MachineSet to Machine", so the arrow points from MachineSet to Machine.

{{< /alert >}}

### KubeadmControlPlane machines relationships

![](/images/kubeadm-control-plane-machines-resources.png)

### Worker machines relationships

![](/images/worker-machines-resources.png)