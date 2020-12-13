# 0013: Backup and restore procedures
- Authors: [David Maas](david_maas@hotmail.de) 
- Status: PROPOSED
- Since: 2020-10-21 
- Status Note: Initial Proposal  
- Start Date: 2020-10-21 
- Tags: 

## Summary
Description of the backup and restore procedure

## Motivation
Due to the decentralised architecture, the data is basically secured and not lost in case of a problem. Nevertheless, the process can be accelerated by backing up the node data and protecting it against misuse. 

## Specification
The following aspects should be observed when backing up and restoring data: 

* Saving the node configuration
* Backup of the node data
* Time interval for the backup
* Automation of the backup routine
* Specify recovery routine
* Node reintegration procedure
* Routine for corrupt data 

## Examples & Best Practices
A possible implementation can be found at [Hyperledger Besu](https://besu.hyperledger.org/en/stable/HowTo/Backup/Backup/): 

>Backups
In a decentralized blockchain, data replicates between nodes so it’s not lost. But backing up configuration and data ensures a smoother recovery from corrupted data or other failures.

>Genesis file
The genesis file for a network must be accessible on every node. We recommend storing the genesis file under source control.

>Data backups
If installed locally, the default data location is the Besu installation directory.

>We recommend mounting a [separate volume to store data](https://besu.hyperledger.org/en/stable/HowTo/Get-Started/Installation-Options/Run-Docker-Image/#starting-besu). Use the [`--data-path`](https://besu.hyperledger.org/en/stable/Reference/CLI/CLI-Syntax/#data-path) command line option to pass the path to Besu.

>The default data location is the Besu installation directory, or `/opt/besu/database` if using the [Besu Docker image](https://besu.hyperledger.org/en/stable/HowTo/Get-Started/Installation-Options/Run-Docker-Image/).

>Having some data reduces the time to synchronize a new node. You can perform periodic backups of the data directory and send the data to your preferred backup mechanism. For example, cron job and rsync, archives to the cloud such as s3, or `tar.gz` archives.

>Data restores
To restore data:

1. If the node is running, stop the node.
2. If required, move the data directory to another location for analysis.
3. Restore the data from your last known good backup to the same directory.
4. Ensure user permissions are valid so you can read from and write to the data directory.
5. Restart the node.

>Corrupted data
If log messages signify a corrupt database, the cleanest way to recover is:

1. Stop the node.
2. Restore the data from a previous backup.
3. Restart the node.

>Finding peers after restarting
The process for finding peers after restarting is the same as for [finding peers after upgrading and restarting](https://besu.hyperledger.org/en/stable/HowTo/Upgrade/Upgrade-Node/#finding-peers-on-restarting).

## Drawbacks
Due to the decentralised architecture, a backup should actually no longer be necessary and thus causes additional effort.

## Prior art

Further information can be found at [Hyperledger Besu Backup and Restore](https://besu.hyperledger.org/en/stable/HowTo/Backup/Backup/)

## Unresolved questions
A standard implementation of backup and distributed data that automatically reconciles and restores the node configuration. Where no manual intervention is required.