Puppet Enviroments for Deploop System
--------------------------------------

    /etc/puppet/environments/
    ├── all
    ├── preproduction
    ├── production
    │   ├── extdata
    │   ├── manifests
    │   │   └── init.pp => include the dedicated clusters (batch, realtime or bus)
    │   └── modules
    │       ├── batch_path
    │       │   └── manifests
    │       │       ├── hadoop_dn.pp => real resource execution from module defines
    │       │       ├── hadoop_nn.pp
    │       │       ├── hadoop_rm.pp
    │       │       ├── hadoop_node.pp
    │       │       └── init.pp => include the host roles
    │       ├── realtime_path
    │       ├── bus_path
    │       ├── hadoop
    │       ├── hbase
    │       ├── kafka
    │       ├── spark 
    │       └── storm
    └── test

Deploop environments Buildoop relation
--------------------------------------

![Image](doc/deploop-environments.jpg?raw=true)
