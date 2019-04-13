# CBT and RCT for VM backup
## What is backup?

Backups is one of the many pain points for system administrators and consequently for their companies. Companies develop and approve retention policies determining backup requirements, procedures, and options, which may vary depending on the needs faced and resources available. Backups of virtual machines expose even higher risks.

As [technopedia determines](https://www.techopedia.com/definition/4805/virtual-machine-vm), a virtual machine (the VM) is a software or an operating system that runs applications and programs as well as performs multiple tasks just as a real computer.

## Overview of Changed Block Tracking (the CBT) and Resilient Change Tracking (the RCT) 

CBT provides for incremental backups. CBT is about tracking and backing up only blocks that changed rather than backing up all the blocks.

*Pic. 1*

![CBT](https://www.google.com/url?sa=i&source=images&cd=&cad=rja&uact=8&ved=2ahUKEwjjjJidmc3hAhVJ-YUKHdjwC7UQjRx6BAgBEAU&url=https%3A%2F%2Fwww.slideshare.net%2Fnakivo%2Fabout-nakivo-2012-1003&psig=AOvVaw1RO8qpR2T3p0ZrRU7G87km&ust=1555249236183690)


