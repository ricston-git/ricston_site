## About coreos

CoreOS provides a new server operating system for running thousands of servers themselves.

[CoreOS](http://coreos.com/) provides a new server operating system for running thousands of servers themselves. CoreOS is designed to give computation capacity that is dynamically scaled and managed, similar to how infrastructure might be managed at large web companies. CoreOS is open source and runs almost anywhere.

CoreOS is designed for security, consistency, and reliability. Instead of installing packages via `yum` or `apt`, CoreOS uses Linux containers to manage your services at a higher level of abstraction. A single service's code and all dependencies are packaged within a container that can be run on one or many CoreOS machines. There are three main building blocks of CoreOS

*   etcd
*   docker
*   systemd

CoreOS runs on almost any platform, including Vagrant, Amazon EC2, QEMU/KVM, VMware and OpenStack and your own hardware. If you're currently running in the cloud, running a single CoreOS cluster on two different clouds or cloud + bare metal is supported and encouraged.

You should use this tag if your question is related to the use of CoreOS or any of its building blocks.