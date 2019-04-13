# CBT and RCT for VM backup
## What is backup?

Backups is one of the many pain points for system administrators and consequently for their companies. Companies develop and approve retention policies determining backup requirements, procedures, and options, which may vary depending on the needs faced and resources available. Backups of virtual machines expose even higher risks.

As [technopedia determines](https://www.techopedia.com/definition/4805/virtual-machine-vm), a virtual machine (the VM) is a software or an operating system that runs applications and programs as well as performs multiple tasks just as a real computer.

## Overview of Changed Block Tracking (the CBT) and Resilient Change Tracking (the RCT) 

CBT provides for incremental backups. CBT is about tracking and backing up only blocks that changed rather than backing up all the blocks.

*Pic. 1*

![CBT](https://sketch.io/render/sk-47b836895052e5b877a8428e085c5d5d.jpeg)


