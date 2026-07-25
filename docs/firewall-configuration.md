# Firewall Configuration

## Objective

Restrict inbound network access to only the services required by the homelab server.

## UFW Installation

UFW was installed and enabled on the Debian server.

The firewall was configured to permit SSH connections only from devices located on the local private network.

## Sanitized Rule

```text
ALLOW TCP PORT 22 FROM 10.0.0.0/24
```

The exact server address has been intentionally omitted.

## Security Benefits

- Blocks unnecessary inbound connections
- Prevents SSH access from outside the approved network range
- Reduces exposure of the server
- Provides a clear and auditable firewall policy

## Verification

The firewall status was checked after configuration.

Remote SSH access from the administration workstation was tested successfully while unauthorized network ranges remained blocked.
