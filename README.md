# CBT and RCT for VM backup
## Let's Start from the Backup: What is It?

Backups is one of the many pain points for system administrators and consequently for their companies. Companies develop and approve retention policies determining backup requirements, procedures, and options, which may vary depending on the needs faced and resources available. Backups of virtual machines expose even higher risks.

As [technopedia determines](https://www.techopedia.com/definition/4805/virtual-machine-vm), a virtual machine (the VM) is a software or an operating system that runs applications and programs as well as performs multiple tasks just as a real computer.

## Breaking Down: Changed Block Tracking (the CBT) and Resilient Change Tracking (the RCT)

CBT provides for incremental backups, which means tracking and backing up only blocks that changed rather than backing up all the blocks.

*Pic. 1*

![CBT](https://sketch.io/render/sk-47b836895052e5b877a8428e085c5d5d.jpeg)

CBT is easy to be implemented: just configure your database and objects. The history of changes, as may be guessed from the name of the approach, is also easy to be tracked. The columns as well as rows that changed may be quickly identified. The performance is high. Context information may be added, if required. And, finally, there is an auto cleanup available: the data collected is deleted based on the date of retention.

However, there are some cons to be mentioned: no tracking of the time of the change; no tracking of security context performing the change; no tracking of the way the data changed; although insignificant, the change adds some overhead to the server; and, what is more, it adds some time to the transaction time.

