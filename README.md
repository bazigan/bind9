# BIND9
DNS Bind9 File Configuration
Include DNS Master-Slave Configuration

Remove additional configuration for the use of a single DNS server in named.conf.default-zones
- Master Server
    allow-transfer{ip-slave;};
    also-notify{ip-slave;};

- Slave Server
    type slave;
    masters{ip-masters;};
