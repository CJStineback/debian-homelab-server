# Debian Installation

## Objective

Convert an older laptop into a dedicated headless Debian Linux server.

## Installation Process

1. Downloaded the Debian network installation image.
2. Created a bootable USB drive using Rufus.
3. Booted the laptop from the installation media.
4. Replaced the previous operating system.
5. Installed Debian without a graphical desktop environment.
6. Selected OpenSSH Server and standard system utilities.
7. Created a non-root administrative account.
8. Configured the system hostname and local networking.
9. Rebooted and verified that Debian started successfully.

## Design Decisions

A graphical desktop environment was not installed because the server is intended to be managed remotely through the command line.

This reduces unnecessary software, resource usage, and potential attack surface.

## Result

The laptop now operates as a dedicated Debian server that can be administered remotely from another Linux workstation.
