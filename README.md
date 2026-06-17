# Redis Cluster Lifecycle Tool with Ansible

## Overview

This project implements a Redis Cluster Lifecycle Tool using Ansible. It provisions a 6-node Redis Cluster, creates the cluster topology, seeds test data, verifies data integrity, monitors cluster status, and supports rolling upgrades with verification.

## Architecture

* 6 Redis Nodes
* 3 Masters
* 3 Replicas
* Redis Cluster Mode Enabled
* Ansible Automation
* Docker-based Environment

### Node Mapping

| Node         | IP         | Role           |
| ------------ | ---------- | -------------- |
| redis-node-1 | 10.10.0.11 | Master/Replica |
| redis-node-2 | 10.10.0.12 | Master/Replica |
| redis-node-3 | 10.10.0.13 | Master/Replica |
| redis-node-4 | 10.10.0.14 | Master/Replica |
| redis-node-5 | 10.10.0.15 | Master/Replica |
| redis-node-6 | 10.10.0.16 | Master/Replica |

## Prerequisites

* Ubuntu Linux
* Docker
* Ansible
* Python3
* SSH Access

## Project Structure

submission/
├── ansible/
├── inventory/
├── playbooks/
├── roles/
├── output/
├── redis-tool
└── README.md

## Features

* Cluster Provisioning
* Cluster Creation
* Status Monitoring
* Data Seeding
* Data Verification
* Full Verification
* Rolling Upgrade Automation

## Commands

### Provision Cluster

./redis-tool provision

### View Status

./redis-tool status

### Seed Data

./redis-tool data seed

### Verify Data

./redis-tool data verify

### Full Verification

./redis-tool verify --full

### Rolling Upgrade

./redis-tool upgrade

## Verification Results

* Cluster State: OK
* Slots Assigned: 16384
* Nodes: 6
* Data Verification: 1000/1000 Keys Verified

## Author

Sruthi B S
B.E Electronics and Communication Engineering
