# Base EE-DE Builder ANY Linux

**Created:** August 2024

## Synopsis

A comprehensive Execution Environment and Decision Engine builder for Ansible Automation Platform. Provides web UI interface for building, managing, and deploying custom execution environments across any Linux distribution with containerized support.

## Supported Operating Systems

- Linux (All distributions with container support)
- Red Hat Enterprise Linux 8/9
- Fedora 35+
- Ubuntu 20.04+
- CentOS Stream 8/9
- Rocky Linux 8/9
- AlmaLinux 8/9

## Quick Usage

### Basic Setup and Execution

```bash
# Run the main setup script
./EE-DE_Builder_WebUI_Install_and_Setup.sh

# Build environments using Ansible
ansible-playbook build_environments.yml

# Configure environment settings
ansible-playbook env_conf.yml

# Start the web interface
make run-frontend

# Run all build processes
make all
```

### Web Interface Access

After setup, access the web interface at:
- Local: http://localhost:3000
- Network: http://your-server-ip:3000

### Command Line Tools

```bash
# Test the structure
./test_structure.sh

# Use Makefile targets
make install        # Install dependencies
make build         # Build all components
make clean         # Clean build artifacts
make test          # Run tests
```

### Interactive Menu System

The web interface provides:

1. Environment Builder Dashboard
2. Execution Environment Management
3. Decision Engine Configuration
4. Container Image Management
5. Build Status Monitoring
6. Log Viewer
7. System Configuration
8. Help and Documentation

## Features and Capabilities

### Core Features

- Web-based user interface for EE/DE management
- Automated installation and setup process
- Cross-platform Linux support with container integration
- Real-time build status monitoring
- Comprehensive logging and error handling
- Desktop integration with launcher creation

### Advanced Features

- Custom execution environment building
- Decision engine template management
- Container image optimization
- Multi-environment support
- Performance monitoring and optimization
- Integration with Red Hat Ansible Automation Platform

### Build System Features

- Makefile-based build automation
- Frontend React/TypeScript application
- Backend API services
- Container orchestration
- Environment configuration management
- Desktop launcher generation

### Integration Components

- Podman/Docker container support
- Ansible Automation Platform integration
- Red Hat Container Registry access
- Custom collection support
- Requirements management
- Template system

## Limitations

- Requires container runtime (Podman or Docker)
- Network connectivity needed for container image downloads
- Requires sufficient disk space for container images and build artifacts
- Some features require Red Hat subscription for official images
- Performance depends on available system resources

## Getting Help

### Documentation

- Check the web interface help section for detailed guides
- Review Makefile targets for available commands
- Examine configuration files in templates/ directory
- Check logs in the web interface or system logs

### Support Resources

- Use the built-in help system in the web interface
- Check container logs for troubleshooting
- Review system requirements before installation
- Verify network connectivity and container registry access

### Common Issues

- Container runtime problems: Ensure Podman/Docker is properly installed
- Network connectivity: Check access to container registries
- Permission issues: Verify user permissions for container operations
- Resource constraints: Monitor disk space and memory usage
- Build failures: Check logs and verify requirements files

## Legal Disclaimer

This software is provided "as is" without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort, or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.

Use this software at your own risk. No warranty is implied or provided.

**By Shadd**
