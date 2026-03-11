# Lima

> Run Linux VMs on macOS with automatic file sharing and port forwarding.

**Platforms:** macOS

## Links
- [Official Website](https://lima-vm.io)
- [GitHub Repository](https://github.com/lima-vm/lima)

## Install

### macOS
```bash
brew install lima
limactl start   # Start the default Ubuntu VM
```

## Usage
```bash
lima uname -a                             # Run a Linux command inside the VM
lima nerdctl run --rm hello-world         # Run a container with containerd
limactl list                              # List VMs
limactl stop default                      # Stop the default VM
```
