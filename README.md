# Lab 9 — Linux Hardening

## Objectives
- Capture before-and-after system snapshots.
- Identify and remove unnecessary services and packages.
- Audit user accounts and login shells.
- Harden SSH and validate configuration before reloading.
- Configure SSH ProxyJump through a router VM.
- Enable and verify automatic security updates.
- Verify exposed ports and SSH authentication.

## Environment
Router LAN interfaces:
- 10.10.10.1/24
- 10.10.20.1/24

SSH uses TCP port 22.

## Repository structure
- `router/` — interfaces, routes, forwarding, and Nmap results.
- `normal-vm/` — snapshots, account audit, SSH configuration, and update logs.
- `client/` — SSH configuration and connection tests.
- `report/` — removal justifications and verification summary.
- `evidence/` — supporting system output.

## Workflow
1. Capture the baseline.
2. Review dependencies and remove unnecessary components.
3. Audit accounts and harden SSH.
4. Validate SSH configuration before reloading.
5. Enable and verify automatic security updates.
6. Capture the final state and compare it with the baseline.
7. Scan the target from the router and test authentication from another host.
