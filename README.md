# Arista Validated Designs using Ansible Automation Platform

This repository is an integration example between [Arista Validated Designs](https://avd.arista.com/), [Ansible Automation Platform](https://www.redhat.com/en/technologies/management/ansible) and [CloudVision](https://www.arista.com/en/products/eos/eos-cloudvision).

It implements the workflow below:

![Arista Validated Designs using Ansible Automation Platform](https://github.com/user-attachments/assets/385e01f5-1cbf-4c50-9e5b-f8472a691735)

The `Update Arista fabric configuration` job aims to build EOS configuration using [AVD](https://avd.arista.com/) and deploy it through CloudVision while the `Test Arista fabric state` job aims to gather and test network states using [ANTA](https://anta.arista.com/) after the network is configured.
