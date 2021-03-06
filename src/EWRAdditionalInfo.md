

### WAN Replication Additional Information

Each cluster in WAN topology has to have a unique `group-name` property for a proper handling of forwarded events.
 
Starting with 3.6, WAN replication backs up its event queues to other nodes to prevent event loss in case of member failures.
WAN replication's backup mechanism depends on the related data structures' backup operations. Note that, WAN replication is supported for IMap and ICache.
That means, as far as you set a backup count for your IMap or ICache instances, WAN replication events generated by these instances are also replicated.
 
There is no additional configuration to enable/disable WAN replication event backups.




