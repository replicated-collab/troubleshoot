---
name: New Production Install
about: Document a new target install scenario for a single end user
title: 'New Installation: [CUSTOMER]'
labels: kind::customer
assignees: ''
---

### Intro, use case, impact, deal value, and target go-live date
<!-- Describe the customer and their use case or value prop. If possible, add any notes on the priority / strategic impact of getting this customer successfully up and running. -->


### Definition of Success
<!-- Define what "success" looks like for this end user, beyond just "getting the software up and running."  Example: we would like to have the customer up and running using our application within 2 weeks of target install time with 10 engineers enabled on the system -->

### Team
- Vendor Technical Leads: 
- Vendor Business Leads:
- Replicated Technical Leads:
- Replicated Business Leads:
- Customer Technical Leads:
- Customer Business Leads:

### Timeline and Next Steps
<!-- Area to Track past engagements as well as next steps. Examples:

- 10/20 Customer identified as potential prospect, PoC kick off scheduled for 10/29
- 10/27 Pre-Planning call with Replicated team, task list reviewed and validated
- 10/29 Initial installation call, app up and running but ran out of disk space and fell over. Replicated team recommends resolving issue [#10 -- preflight checks for disk space]() before next attempt.
- 11/01 Customer working to provision new machine with bigger disk, next attempt 11/3
 -->

### Environment
<!-- Describe the customer’s environment-->

**Install type:**
<!-- Is this an Embedded or Existing Cluster? -->

**Airgap:**
<!-- Is this an Airgapped and/or BYO Registry installation? -->

**Registry:**
<!-- Will images be used from public container registries like Dockerhub or Quay.io? If this is airgapped, will we use kURL's embedded registry or will the customer bring their own registry?  Does the registry we decide to use require authentication? --> 

**Operating System** (if embedded cluster):
<!-- Red Hat, Centos, Ubuntu, etc -->

**Cluster Topology** (if embedded cluster):
<!-- How many nodes are used, in what roles? Is this a Highly Available (HA) Kubernetes installation? -->

**Cluster Flavor / K8s version** (if existing cluster):
<!-- Amazon EKS, Openshift, Tanzu, kops, etc, version 1.24.1-->

**Ingress Strategy:**
<!-- How will the end user interact with the application and with the app manager UI? Will there be a load balancer in front of a VM? Do they have an existing ingress or service mesh controller that must be used? Do any services require Node Ports? -->

**Storage:**
<!-- Does this customer require special considerations for planning storage?  For instance, are they going to provision separate partitions for /var, /var/lib/docker, /var/lib/containerd, /var/lib/kubelet, etc.  or do they plan to use a single large partition?   How much space will be available?  What process is required to get additional storage if that is required?  -->

**Security & Access:**
<!-- Does the customer have root access to the environment?  If using an existing cluster, do they require minimal RBAC roles?  If using an embedded cluster, do they have root access to the VM we will use?  If using an embedded cluster, would they be able to provision additional resources as may be required (firewall changes, load balancer rules, storage partitions, etc.) or is there a change request process that must be followed? -->

**Datacenter:**
<!-- is the datacenter on prem, in the cloud? if it's on prem, is it VMs on VMWare, bare metal, etc.?  If it's cloud based, AWS, Azure, etc.? -->

**Additional Details:**
<!-- Any other details to note? -->

### Additional Tasks Required to Prepare for this installation
<!-- Can include integration work from Packaging board, testing work, documentation work, planning calls or anything else. 
  The below is meant to outline the bare minimum and is should be extended. -->

- [ ] Discovery: Outline [Customer Environment](#environment)
- [ ] Schedule Installation Date: 
- [ ] Schedule pre-install huddle with Replicated CS team
- [ ] Create (and test in) a representative internal test environment based on information about [Customer Environment](#environment)
