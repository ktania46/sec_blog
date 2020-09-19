---
layout: post
title:  "Introduction"
date:   2020-09-19 18:02:43 +0530
categories: jekyll update
---
Red Hat and IBM Power teams have been working together on OpenShift since 2018 with the initial release of OpenShift 3.11 on Power. Through this continuous collaboration and effort between IBM and Red Hat, improvements on Power have been made such as the support of IBM PowerVM with OpenShift to enable our Power Enterprise systems. OpenShift on IBM Power Systems takes advantage of the Hybrid Cloud Flexibility, as a result of it, OpenShift can be deployed on PowerVM or Red Hat KVM (development) on Power scale-out servers to exploit the 3.2x container density advantage per core of the POWER9 multi-threaded architecture. Automation for OpenShift on IBM Power Architecture can make things easier and much faster for the end user, making the entire process hasslefree allowing Power clients to exploit the innovative new capabilities.A deployment host is any virtual or physical host that is typically required for the installation of Red Hat OpenShift. The Red Hat OpenShift installation assumes that many, if not all the external services like DNS, load balancing, HTTP server, DHCP are already available in an existing data center and therefore there is no need to duplicate them on a node in the Red Hat OpenShift cluster. Master node, worker node and bootstrap can run on top of PowerVC, PowerVM, Red Hat Virtualization, KVM or run bare metal environments. You can manage trust configuration directly on each node or manage the files on a separate host by distributing them to the appropriate nodes using Ansible.

Ansible is an automation tool used to configure systems, deploy software, and perform rolling updates. Ansible includes support for container-native virtualization, and Ansible modules enable you to automate cluster management tasks such as template, persistent volume claim, and virtual machine operations. Ansible provides a way to automate container-native virtualization management, which you can also accomplish by using the `oc` CLI tool or APIs. Ansible is unique because it allows you to integrate KubeVirt modules with other Ansible modules.


Playbooks are Ansible’s configuration, deployment, and orchestration language. They can describe a policy you want your remote systems to enforce, or a set of steps in a general IT process. If Ansible modules are the tools in your workshop, playbooks are your instruction manuals, and your inventory of hosts are your raw material.
At a basic level, [playbooks][playbooks] can be used to manage configurations of and deployments to remote machines. At a more advanced level, they can sequence multi-tier rollouts involving rolling updates, and can delegate actions to other hosts, interacting with monitoring servers and load balancers along the way.
Playbooks are designed to be human-readable and are developed in a basic text language. There are multiple ways to organize playbooks and the files they include.
The Playbooks are used for installation of OCP on Power and other post install customizations

[Terraform][terraform] is an Open Source software that is developed by HashiCorp that enables predictable and consistent provisioning of IBM Cloud platform, classic infrastructure, and VPC infrastructure resources by using a high-level scripting language. Terraform is used to create, manage, and update infrastructure resources such as physical machines, VMs, network switches, containers, and more. Terraform can be used to automate IBM Cloud resource provisioning, rapidly build complex, multi-tier cloud environments, and enable Infrastructure as Code (IaC).

A lot of OpenShift 4 specific jargon is used throughout this doc, so please visit the [official documentation page][official documentation page] to get familiar with OpenShift 4.

[playbooks]: https://github.com/ocp-power-automation/ocp4-playbooks
[terraform]: https://www.terraform.io/docs/providers/index.html
[official documentation page]: https://docs.openshift.com/container-platform/latest


