ansible-role-beegfs-client
=========

Simple role installing the beegfs client in a CentOS machine

NO RDMA SUPPORT BY NOW

Requirements
------------

None

Role Variables
--------------

```
beegfs_version: 7.1.2

beegfs_master_server: 192.168.200.251

beegfs_add_repos: True

beegfs_repo_url: "https://www.beegfs.io/release/latest-stable/dists/beegfs_rhel7.repo"

beegfs_repo_key: "https://www.beegfs.io/release/latest-stable/gpg/RPM-GPG-KEY-beegfs"

beegfs_repo_file: "/etc/yum.repos.d/beegfs-rhel7.repo"

beegfs_network_interface: eno2
```

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ansible-role-beegfs-client }

License
-------

GPLv3

Author Information
------------------

Pablo Escobar
