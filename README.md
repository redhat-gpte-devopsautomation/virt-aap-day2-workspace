# virt-aap-day2-workspace

Welcome to the **virt-aap-day2-workspace** repository! This repository is
designed to support **Day 2 operations** for Virtual Machines (VMs) on OpenShift
Virtualization using **Ansible Automation Platform (AAP)**. It contains all
the necessary playbooks and roles to manage, patch,
and maintain VMs effectively in a dynamic OpenShift environment.

## Repository Structure

This repository is organized to provide clear guidance on automating Day 2 operations:

- **Roles**:
  - `vm_management`: A role for managing VM lifecycle operations such as stopping, starting, and restarting VMs.

- **Playbooks**:
  - `manage_vm_playbook.yml`: Executes VM lifecycle operations.
  - `patch_vm_playbook.yml`: Applies security updates to RHEL-based VMs.
  - `backup_restore_vm_playbook.yml`: Backs up and restores VMs.

- **Dynamic Inventory Configuration**:
  - Details to create an AAP inventory  to dynamically integrate OpenShift-hosted VMs into Ansible Automation Platform (AAP).

## Features

- **Lifecycle Management of VMs**:
  Automate starting, stopping, and restarting VMs using the `redhat.openshift_virtualization` Ansible Collection.

- **Security Patch Management**:
  Apply critical security updates to your RHEL-based VMs using the `dnf` module.

- **Dynamic Inventory**:
  Manage OpenShift Virtualization VMs dynamically within AAP, enabling automation that adapts to changes in your infrastructure.

- **Backup and Restore**:
  Protect workloads by creating backups of VMs and restoring them when necessary.

## Getting Started

### Prerequisites

- **Ansible Automation Platform**: Ensure AAP is installed and configured.
- **Execution Environment**: Use the prebuilt `Day2 EE` containing required collections (`redhat.openshift_virtualization`, `redhat.openshift`).
- **Access to OpenShift Cluster**: Ensure you have the necessary credentials and access to your OpenShift cluster.

### How to Use This Repository

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/virt-aap-day2-workspace.git
   cd virt-aap-day2-workspace


### Hands-on Workshop

For Red Hatt employees and Red Hat partners you can order this workshop via [demo.redhat.com](demo.redhat.com).  The workshop catalog item is [Operations and Automation with OpenShift Virtualization
](https://catalog.demo.redhat.com/catalog?item=babylon-catalog-prod/openshift-cnv.virt-aap-day-2.prod&utm_source=webapp&utm_medium=share-link).  The showroom (lab directions) can be found here: [https://rhpds.github.io/showroom-virt-aap-day-2/modules/index.html](https://rhpds.github.io/showroom-virt-aap-day-2/modules/index.html)

For an entire lab listing of all Ansible Automation Platform workshop, please look here: [https://labs.demoredhat.com/](https://labs.demoredhat.com/).

### Red Hat Ansible Automation Platform

Turn automation into your strategic advantage with [Red Hat® Ansible® Automation Platform](https://redhat.com/ansible). Gain a trusted, versatile solution that can tackle any use case, run anywhere, and bring out the automator in everyone.

![logo ansible automation platform](images/logo_aap.png)