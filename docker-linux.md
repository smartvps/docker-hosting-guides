# Docker on Linux: Installation and Management Guide

Linux provides a native environment for Docker containers and is widely used for containerized applications on VPS, VDS and dedicated servers.

This guide covers Docker installation options across popular Linux distributions, basic configuration and container management.

## Supported Linux Distributions

Docker Engine is available for various Linux distributions, including:

- Ubuntu
- Debian
- CentOS Stream
- Fedora
- Red Hat Enterprise Linux (RHEL)

Installation methods and supported releases vary depending on the distribution.

## System Requirements

Before installing Docker, make sure your server has:

- A compatible Linux distribution and kernel.
- Sufficient CPU and RAM for your workloads.
- Available disk space for images, containers and volumes.
- Root or sudo access.
- Compatible virtualization technology.

## Docker on Ubuntu 26.04

Ubuntu is a popular choice for running Docker on virtual and dedicated servers.

For release-specific installation instructions, follow the [Docker installation guide for Ubuntu 26.04](https://smartvds.org/software-setup-guides/install-docker-ubuntu-26-04/).

## Docker on Ubuntu and Debian

Debian-based distributions provide a stable environment for containerized applications and server infrastructure.

Read the [Docker installation guide for Ubuntu and Debian](https://smartvds.org/software-setup-guides/docker-ubuntu-debian-guide/) for detailed setup instructions.

## Docker on CentOS, Fedora and RHEL

RPM-based distributions use different package management tools and repository configurations.

Follow the [Docker guide for CentOS, Fedora and RHEL](https://smartvds.org/software-setup-guides/docker-centos-fedora-rhel-guide/) for distribution-specific installation instructions.

## Verifying Docker Installation

Check the Docker version:

```bash
docker --version
```

Check the Docker service status:

```bash
sudo systemctl status docker
```

Run a test container:

```bash
sudo docker run --rm hello-world
```

Check Docker Compose availability:

```bash
docker compose version
```

## Security and Maintenance

- Keep the Linux operating system updated.
- Regularly update Docker Engine and container images.
- Review exposed ports and firewall configuration.
- Avoid unnecessary privileged containers.
- Restrict access to the Docker socket.
- Maintain backups of persistent volumes.
- Monitor CPU, memory and storage usage.

## Related Guides

- [Docker General Guide](./docker-guide.md)
- [Docker on Windows](./docker-windows.md)
- [Docker & Portainer](./docker-portainer.md)

---

[Back to Docker Hosting Guides](./README.md)
