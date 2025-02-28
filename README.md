# Arista Validated Designs using Ansible Automation Platform

This repository is an integration example between [Arista Validated Designs](https://avd.arista.com/), [Ansible Automation Platform](https://www.redhat.com/en/technologies/management/ansible) and [CloudVision](https://www.arista.com/en/products/eos/eos-cloudvision).

It implements the workflows below:

![Arista Validated Designs using Ansible Automation Platform](https://github.com/user-attachments/assets/298b1f01-8f81-4920-ae09-a480203d3546)

The `Update Arista fabric configuration` job aims to build EOS configuration using [AVD](https://avd.arista.com/) and deploy it through CloudVision while the `Test Arista fabric state` job aims to gather and test network states using [ANTA](https://anta.arista.com/) after the network is configured.

The network topology used is represented by the following diagram:

![avd-aap](https://github.com/user-attachments/assets/1391c1c3-83f6-475c-add2-05e0439a5ed9)
