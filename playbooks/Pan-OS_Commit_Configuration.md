---
id: pan-os-commit-configuration
title: Pan-OS Commit Configuration
---

Commits the PAN-OS Panorama or Firewall configuration. If specified as Panorama, it also pushes the policies to the specified device group in the instance.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
* GenericPolling

### Integrations
* Panorama

### Scripts
This playbook does not use any scripts.

### Commands
* panorama
* panorama-commit-status
* panorama-push-status
* panorama-push-to-device-group
* panorama-commit

## Playbook Inputs
---
There are no inputs for this playbook.

## Playbook Outputs
---
There are no outputs for this playbook.

![Pan-OS_Commit_Configuration](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/PAN-OS_Commit_Configuration.png)
