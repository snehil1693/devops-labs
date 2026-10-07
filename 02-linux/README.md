# 02 · Linux

Covers Linux core concepts (filesystem hierarchy, file types and inodes, permissions incl. SUID/SGID/sticky and ACLs, users/groups and least-privilege sudo, processes and signals, file descriptors, systemd services and timers, the boot process) and Linux operations (disks, fstab, LVM, memory and the OOM killer, CPU/load, disk I/O, logs and logrotate, cron, SSH bastions/tunnels/hardening, performance triage with the USE method).

Lab environment: a local Ubuntu 24.04 VM via Multipass (`multipass launch 24.04 --name devops-lab`).

| Lab | Level | What I built / learned | File(s) | Done |
|---|---|---|---|---|
| 5.1 | 🟢 | Explore kernel, distro, FHS, file types, hard vs soft links, inodes | `lab-5.1-explore.md` | ⬜ |
| 5.2 | 🟢 | Permissions, umask, SUID audit, reproduce and fix an Nginx 403 | `lab-5.2-permissions.md` | ⬜ |
| 5.3 | 🟡 | Users, groups, SGID+sticky team dir, least-privilege sudoers | `lab-5.3-users-sudo.md` | ⬜ |
| 5.4 | 🟡 | Processes and signals: trap/graceful shutdown, jobs, zombies, /proc | `lab-5.4-processes-signals.md`, `graceful.sh` | ⬜ |
| 5.5 | 🔴 | **Hardened systemd service** (non-root, auto-restart, env file) + health-check **timer** | `lab-5.5-systemd/` | ⬜ |
| 5.6 | 🔴 | **Linux security & health audit script** (UID 0, sudo, SUID, perms, failed units, zombies, disk/inodes, deleted-open files) | `linux_audit.sh` | ⬜ |
| 6.1 | 🟢 | Disks and usage: lsblk/df/du/ncdu, inode exhaustion, reproduce + fix the deleted-but-open leak | `lab-6.1-disks.md` | ⬜ |
| 6.2 | 🟢→🟡 | LVM across two disks, fstab by UUID + `nofail`, grow online, LVM snapshot restore | `lab-6.2-lvm.md` | ⬜ |
| 6.3 | 🟡 | CPU / I/O / memory pressure with stress-ng, reading vmstat/iostat/mpstat, OOM killer, swap, systemd `MemoryMax` | `lab-6.3-mem-cpu-oom.md` | ⬜ |
| 6.4 | 🟡 | Log app with SIGHUP reopen, logrotate (create vs copytruncate), persistent journald, safe cron with `flock` | `lab-6.4-logs-cron/` | ⬜ |
| 6.5 | 🔴 | **SSH like a pro**: bastion + ProxyJump, local tunnel, sshd hardening drop-in, fail2ban | `lab-6.5-ssh/` | ⬜ |
| 6.6 | 🔴 | **`triage.sh`**: "first 60 seconds" incident triage tool (USE method, Ubuntu + Amazon Linux, `--json`) | `triage.sh` | ⬜ |
