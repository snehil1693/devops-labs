# 02 · Linux

Covers Linux core concepts: filesystem hierarchy, file types and inodes, permissions (incl. SUID/SGID/sticky, ACLs), users/groups and least-privilege sudo, processes and signals, file descriptors, systemd services and timers, and the boot process.

Lab environment: a local Ubuntu 24.04 VM via Multipass (`multipass launch 24.04 --name devops-lab`).

| Lab | Level | What I built / learned | File(s) | Done |
|---|---|---|---|---|
| 5.1 | 🟢 | Explore kernel, distro, FHS, file types, hard vs soft links, inodes | `lab-5.1-explore.md` | ⬜ |
| 5.2 | 🟢 | Permissions, umask, SUID audit, reproduce and fix an Nginx 403 | `lab-5.2-permissions.md` | ⬜ |
| 5.3 | 🟡 | Users, groups, SGID+sticky team dir, least-privilege sudoers | `lab-5.3-users-sudo.md` | ⬜ |
| 5.4 | 🟡 | Processes and signals: trap/graceful shutdown, jobs, zombies, /proc | `lab-5.4-processes-signals.md`, `graceful.sh` | ⬜ |
| 5.5 | 🔴 | **Hardened systemd service** (non-root, auto-restart, env file) + health-check **timer** | `lab-5.5-systemd/` | ⬜ |
| 5.6 | 🔴 | **Linux security & health audit script** (UID 0, sudo, SUID, perms, failed units, zombies, disk/inodes, deleted-open files) | `linux_audit.sh` | ⬜ |
