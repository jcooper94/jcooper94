# Virtual Networks

## Network function virtualization (NFV)
Replace physical network devices with virtual versions

Same funcitonality as the physical setup
- Routing, Switching, Load Balacning, Firewalls, etc.

# Hypervisor

**Virtual Machine Manager**
Manages the virtual platform and guest operating systems. Provides hardware management for CPU, networking, security, all accessible through a single console control.

## Type 1 Hypervisors (Bare Metal Hypervisors):
- VMware ESXi
- Proxmox
- Microsoft Hyper-V Server
- Citrix Hypervisor (formerly XenServer)
- KVM (Kernel-based Virtual Machine)

## Type 2 Hypervisors (Hosted Hypervisors):
- VMware Workstation
- Oracle VirtualBox
- Microsoft Hyper-V (when installed on Windows Desktop)
- Parallels Desktop for Mac

# vSwitch
Virtual switch
Move the physical switch into the virtual environment
Functionality is similar to a physical switch
Forwarding options
Link aggregation
Port mirroring
NetFlow

# vNIC
A virtual networking interface card
VLAN, aggregation, multiple interfaces