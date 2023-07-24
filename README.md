# BIND9
DNS Bind9 File Configuration
Include DNS Master-Slave Configuration

Delete additional configuration in named.conf.default-zones
- Master Server
* allow-transfer{ip-slave;};
* also-notify{ip-slave;};

- Slave Server
* type slave;
* masters{ip-masters;};
