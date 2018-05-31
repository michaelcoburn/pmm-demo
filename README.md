# PMM Demo
Set up a multi-server & technologies under load. Powers [Percona Monitoring and Management Demo|https://pmmdemo.percona.com]

# Environment
- Percona Server for MySQL 5.5, 5.6, 5.7
  - Engines: TokuDB, MyRocks
- MySQL Community 5.7, 8.0
- PXC 5.7
- ProxySQL
- Percona Server for MongoDB
  - Engines: mmapv1, memory, WiredTiger, RocksDB
- PostgreSQL 10
- MariaDB 10.3
- MongoDB 3.6

## TODO
- PostgreSQL 10 workload generation, pmm-client
- MySQL 5.7, 8.0 workload generation, pmm-client
- ProxySQL
- PXC
- Percona Server for MongoDB 3.6
- MongoDB 3.6

## Usage
Set up your DigitalOcean API key as an environment variable:
```
export DO_API_TOKEN=$(cat ~/DO-personal-access-token)
```
Run the master playbook
```
ansible-playbook main.yml
```
Created by @PeterZaitsev, added by @delgod, @michaelcoburn
