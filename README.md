# Docker Sec Auditor

![Security](https://img.shields.io/badge/Security-Tool-red)
![Bash](https://img.shields.io/badge/Bash-Script-green)
![Docker](https://img.shields.io/badge/Docker-Container-blue)
![License](https://img.shields.io/badge/License-MIT-blue)

A Docker container security auditing tool that inspects running containers, images, and configurations for security misconfigurations and vulnerabilities.

## Description

Docker Sec Auditor performs automated security assessments of Docker environments. It checks for common misconfigurations such as running containers as root, exposed ports, insecure volume mounts, and outdated base images. Designed to integrate into CI/CD pipelines for continuous container security.

## Features

- Audit running Docker containers for security issues
- Check Dockerfiles for best practice violations
- Detect containers running with elevated privileges
- Identify exposed ports and insecure network configurations
- Scan for outdated or vulnerable base images
- System-level hardening baseline checks
- Makefile-based build and test workflow

## Tech Stack

- **Language:** Bash
- **Platform:** Docker
- **Target OS:** Linux
- **Build Tool:** GNU Make

## Quick Start

```bash
# Clone the repository
git clone https://github.com/razinahmed/docker-sec-auditor.git
cd docker-sec-auditor

# Review the auditing script
cat scripts/security_core.sh

# Run the Docker security audit
sudo bash scripts/security_core.sh
```

## Usage

```bash
# Build and test
make build
make test

# Run the security audit
sudo bash scripts/security_core.sh
```

## Project Structure

```
docker-sec-auditor/
  scripts/
    security_core.sh  # Core Docker auditing script
  Makefile             # Build and test automation
  SECURITY.md          # Security policy
  LICENSE              # MIT License
```

## Contributing

Contributions are welcome. Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
