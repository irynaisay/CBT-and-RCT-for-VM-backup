# CBT and RCT for VM Backup

Nowadays, there are many backup solutions. Some of them are leverage technologies. However, that’s not what we are here today for: we won’t do any estimations and we won't rank solutions available in the market. To stay up-to-date with the market developments, we'll check on CBT and RCT in general.

## What is Backup for VMs?

Backups is one of the many pain points for system administrators and consequently for their companies. Businesses develop and approve retention policies determining backup requirements, procedures, and options that vary depending on the needs faced and resources available. Backups of virtual machines expose even higher risks.

As [technopedia determines](https://www.techopedia.com/definition/4805/virtual-machine-vm), a virtual machine (the VM) is a software or an operating system that runs applications and programs as well as performs multiple tasks just as a real computer.

Backups of VMs are essential to protect data. Today, with heavy loads on servers, there are many nicee backup tools that allow mainstreaming myriads of sophisticated tasks. Let's take a lookt at them.

## Breaking Down: CBT and RCT

**Changed Block Tracking (the CBT)** provides for incremental backups, which means tracking and backing up only blocks that changed rather than backing up all the blocks. 

*Pic. 1*

![CBT](https://sketch.io/render/sk-47b836895052e5b877a8428e085c5d5d.jpeg)

CBT is easy to be implemented: just configure your database and objects. The history of changes, as may be guessed from the name of the approach, is also easy to be tracked. The columns as well as rows that changed may be quickly identified. Some context information may be added, if required. And, finally, there is an auto cleanup available: the data collected is deleted based on the date of retention.

However, there are some cons to be mentioned: no tracking of the time of the change; no tracking of security context performing the change; no tracking of the way the data changed; although insignificant, a change may add some overhead to the server; and, what is more, it does add some time to the transaction time.

As Microsoft had no CBT-like feature, in 2016, with the release of Windows Server 2016, they introduced their **Resilient Change Tracking (the RCT)**. RCT allows tracking changes that occur between backup sessions. The changed blocks are the candidates for backing up.

What makes users so excited about RCT, you may ask. Well, Microsoft offers Modified Region Table (the MRT), which maintains records of changes with the disk or the storage. Therefore, you don’t have to fully rescan the disk/storage for changes. In addition, the RCT file capacity is up to 6MB. It may be used for migrations, for instance.

Of course, there are cons in the RCT approach. However, the built-in technology runs faster and more efficiently with every new release, the gaps are getting filled and businesses are strengthening their backing up forces.

If you want to learn details, [here](https://www.nakivo.com/blog/vm-backup-hyper-v-changed-block-tracking-cbt/) is a description of how the RCT works.
