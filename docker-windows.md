# Docker on Windows: Installation and Management Guide

Docker provides a flexible environment for developing, deploying and managing containerized applications on Windows desktop and server operating systems.

## Windows Container Environments

Docker-related container technologies can be used on:

- Windows Server 2022
- Windows Server 2025
- Windows 10
- Windows 11

Installation methods and runtime requirements differ between Windows Server and desktop editions.

## System Requirements

Before installing a container runtime, consider:

- Operating system version and compatibility.
- Hardware virtualization support.
- Available CPU, RAM and disk space.
- Administrative privileges.
- WSL 2 or Hyper-V requirements.
- Nested virtualization support when using a virtual server.

## Docker on Windows Server 2022 and 2025

Windows Server provides an environment for running Windows containers and deploying enterprise applications.

Unlike desktop operating systems, Windows Server requires a compatible server container runtime. Docker Desktop is not supported on Windows Server.

For detailed instructions, read the [Docker installation guide for Windows Server 2022 and 2025](https://smartvds.org/windows/install-docker-windows-server-2022-2025/).

## Docker on Windows 10 and 11

Docker Desktop simplifies container management and application development on supported Windows desktop systems.

Using the WSL 2 backend, developers can run Linux containers alongside their Windows applications.

Follow the [Docker installation guide for Windows 10 and 11](https://smartvds.org/windows/install-docker-windows-10-11/) for platform-specific configuration instructions.

## Windows Containers vs Linux Containers

| Feature | Windows Containers | Linux Containers |
|---|---|---|
| Environment | Windows kernel | Linux kernel |
| Common workloads | Windows-based applications | Web services, databases and APIs |
| Typical use | Windows infrastructure | Development and server hosting |

## Verifying Docker Installation

Check the installed Docker version:

```powershell
docker --version
```

Display Docker environment information:

```powershell
docker info
```

List running containers:

```powershell
docker ps
```

Check Docker Compose availability:

```powershell
docker compose version
```

## Security and Maintenance

- Keep Windows and container runtimes updated.
- Use trusted container images.
- Restrict unnecessary network access.
- Monitor container resource consumption.
- Back up persistent application data.
- Verify container image compatibility before deployment.

## Related Guides

- [Docker General Guide](./docker-guide.md)
- [Docker on Linux](./docker-linux.md)
- [Docker & Portainer](./docker-portainer.md)

---

[Back to Docker Hosting Guides](./README.md)
