Until the late 1990s, applications developed by a company were tightly coupled with its hardware - they couldn't run on another vendor's hardware, or across operating systems.

..that is until virtualization technology became popular and widely used

A 🧵 on virtual machines:

A virtual machine or virtual computer system is an isolated software container with its own operating system and applications inside.

One physical system (such as your laptop) can 'host' one or more VMs. The physical system is known as the "host", while each VM is a "guest".
1/n

With VMs you can use physical servers more efficiently - if one of your tasks is not using a server entirely, you can add a VM to the server and use it for another task.

You can also run multiple operating systems (e.g. Linux and MacOS) on the same physical machine with VMs.
2/n

The technology behind VMs - virtualization - has existed for several decades.

"Virtualization is the process of creating a software-based (virtual) version of something, whether that be compute, storage, networking, servers or applications."
3/n

VMware explains beautifully the benefits of virtualization:

a) Partitioning: Run multiple operating systems on one physical machine 

4/n

b) Isolation:
Each VM is a tightly isolated software container with its own operating system and applications inside. VMs provide fault and security isolation.

5/n

c) Encapsulation:
The state of virtual machine is stored in files. You can move and copy VMs from one physical system to another as easily as copying files.

d) Hardware Independence
Provision or migrate any VM to any physical server

6/n

A piece of software called "Hypervisor" makes virtualization possible.

A Hypervisor pools resources, such as compute power and storage, from the physical server and allocates them to VMs. 7/n

Hypervisors also manage the scheduling of VM resources against physical resources - think of a sports coach that has to allow his class of 30 play on the field when only 5 can play at a time. He has to set out the schedule for play and ensure each student gets a chance. 8/n

When the virtual environment is running and a user or program issues an instruction that requires additional resources from the physical environment, the hypervisor relays the request to the physical system and caches the changes—which all happens at close to native speed. 9/n

There are 2 kinds of Hypervisors:
Type 1 or "bare-metal hypervisors" are installed directly on the physical system. They take the place of the host OS and directly schedule VM resources to the hardware. These are more secure, have low latency and are frequently used. 10/n

KVM, or Kernel Virtual Machine, is a Type 1 Hypervisor that is open-source and part of the Linux Kernel. Since 2007, it is pre-installed as part of Linux distributions. 

Most enterprise, especially data centres, use Type 1 hypervisors. 11/n

Type 2 or "Hosted" Hypervisors are a separate software layer that is installed on an operating system (the hypervisor is hosted on the machine's primary OS).

Type 2 Hypervisor > Host Operating System > Physical server (where > can be read as "on top of") 

 12/n

Individual users run multiple Operating systems on a single machine using Type 2 Hypervisors such as VMWare and VirtualBox. 

Since communication must pass through the additional layer of the host operating system, Type 2 Hypervisors have higher latency than Type 1. 13/n


We can see that virtual machines:
a) help save on cost - you need less physical servers 
b) improve development speed - develop on Mac, but test on Windows or Linux with VMs
c) reduce downtime - if one physical server isn't working, move your VMs to another machine. 14/n


Resources:
https://www.vmware.com/topics/glossary/content/hypervisor.html
https://www.vmware.com/in/solutions/virtualization.html
https://www.ibm.com/cloud/learn/virtualization-a-complete-guide
https://www.ibm.com/cloud/learn/virtual-machines
https://www.redhat.com/en/topics/virtualization/what-is-a-hypervisor
https://www.redhat.com/en/topics/virtualization/what-is-virtualization
https://www.redhat.com/en/topics/virtualization
https://www.redhat.com/en/topics/containers/containers-vs-vms
https://www.redhat.com/en/topics/cloud-computing/cloud-vs-virtualization


