# SSH Hardening

## Objective

Secure remote administration of the Debian server using SSH public-key authentication.

## Key Generation

An SSH key pair was generated on the Linux Mint administration workstation.

The private key remains only on the administration device. The public key was installed on the Debian server.

## Authentication Testing

Key-based authentication was tested successfully before password authentication was disabled.

This prevented accidental loss of remote access.

## OpenSSH Security Controls

The following settings were applied:

```text
PermitRootLogin no
PasswordAuthentication no
KbdInteractiveAuthentication no
PubkeyAuthentication yes
```

Access was restricted to an authorized administrative account.

## Security Benefits

- Prevents direct SSH login as root
- Removes remotely guessable account passwords
- Requires possession of an authorized private key
- Reduces exposure to password-based brute-force attacks
- Limits remote administration to an approved account

## Verification

A second SSH session was opened after the changes were applied to verify that key authentication still worked.

The original session remained open until the new configuration was confirmed.
