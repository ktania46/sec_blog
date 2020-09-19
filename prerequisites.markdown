---
layout: page
title:  Prerequisites
permalink: /prerequisites1/
---
* Git: Please refer to the [link](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) for instructions on installing the latest Git.

* [Go](https://golang.org/doc/install) 1.13 (to build the provider plugin)

* [Preparing Images for Power](https://github.com/ocp-power-automation/ocp4-upi-kvm/blob/master/docs/prepare-images.md)

* docker v17.03+, podman v1.2.0+, or buildah v1.7+

* Access to a cluster based on Kubernetes v1.12.0+

* Access to a container registry

* Public internet connection for all the nodes to download the playbooks and images as part of the setup process.
VM configs for OpenShift nodes that will be deployed with RHCOS image.

* Bootstrap, Master - 4 vCPUs, 16GB RAM, 120 GB Disk
This config is suitable for majority of the scenarios

* Worker - 4 vCPUs, 16GB RAM, 120 GB Disk
Increase worker vCPUs, RAM and Disk based on application requirements

Following is the recommended VM config for the helper node that will be deployed with RHEL 8.0 (or later) image.

* Helper node (bastion) - 2vCPUs, 16GB RAM, 200 GB Disk 

