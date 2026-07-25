# Lessons Learned

## SSH Key Management

I learned the difference between an SSH public key and private key.

The public key can be installed on systems that I need to access. The private key must remain protected and should never be uploaded or shared.

## Safe Configuration Changes

I learned to keep an existing SSH session open while testing security changes in a second session. This reduces the risk of locking myself out of the server.

## Firewall Rules

I learned that allowing SSH from anywhere is less secure than restricting access to the local private network.

I removed overly broad rules and replaced them with a rule limited to the home network range.

## Headless Administration

I gained experience managing a Linux system without a graphical interface, including installing packages, editing configuration files, checking services, configuring networking, and shutting down the machine remotely.

## Troubleshooting

The project required troubleshooting installation media, boot options, SSH authentication, firewall rules, permissions, and remote connectivity.

Working through these issues improved my ability to diagnose problems systematically.
