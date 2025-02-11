# Cloud Instance Initialization

A Vagrant-based development environment setup with automated cloud initialization for Docker and Grafana.

## Description

This project provides an automated setup for a development environment using Vagrant and cloud-init. It creates an Ubuntu 20.04 LTS virtual machine with pre-configured Docker and Grafana installations.

## Features

- Automated VM provisioning using Vagrant
- Ubuntu 20.04 LTS base system
- Pre-installed packages:
  - Docker CE with proper MTU configuration
  - Grafana
  - System utilities (neofetch, htop)
- Automated user setup with Docker permissions
- Preconfigured port forwarding (3000)
- 8GB RAM allocation

## Prerequisites

- VirtualBox
- Vagrant
- Sufficient disk space and RAM

## Quick Start

1. Clone this repository
2. Run `vagrant up` in the project directory
3. The VM will initialize with all configurations
4. Access Grafana through `http://localhost:3000`

## Configuration Details

### Vagrant Configuration
- Port 3000 forwarded for Grafana access
- 8GB RAM allocated
- Cloud-init integration for automated setup

### Cloud-Init Features
- Docker repository configuration
- Grafana repository setup
- Automated package installation
- Docker MTU configuration
- User creation with Docker permissions
- Service automation (Docker and Grafana)

### Pre-configured Users
- Two users (Mallory and Eve) with Docker permissions
- Preconfigured with secure password hashes
- Shell access enabled

## Usage

```bash
# Start the VM
vagrant up

# SSH into the VM
vagrant ssh

# Stop the VM
vagrant halt

# Remove the VM
vagrant destroy
```

## Service Access

- Grafana: http://localhost:3000
  - Default credentials: admin/admin

## Project Status

Active development - Production ready

## License

This project is licensed under the MIT License
