# Galera Replication Overview

Data replication in a Galera cluster is handled via the Write Set Replication API

* wsrep is the core mechanism that enables synchronous and multi-master replication 
* wsrep intercepts database transactions, packages them into write-sets, and then distributes them to all nodes for certification and simultaneous application