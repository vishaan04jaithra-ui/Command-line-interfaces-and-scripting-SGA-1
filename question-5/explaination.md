 # Linux Storage Health Assessment

This task evaluates the storage status of the Linux system by examining storage devices, mounted filesystems, disk usage, and inode utilization.

---

## Commands Used

### 1. Display Storage Devices

```bash
lsblk
```

Lists all available storage devices, partitions, and mount points.

---

### 2. Check Disk Usage

```bash
df -h
```

Displays disk usage information in a human-readable format.

The output includes:

- Filesystem
- Total Size
- Used Space
- Available Space
- Usage Percentage
- Mount Point

---

### 3. Check Inode Utilization

```bash
df -i
```

Displays inode usage statistics for all mounted filesystems.

This helps determine whether the filesystem is approaching its inode limit.

---

## Observations

- The primary storage device is **sda**.
- The root partition is mounted on **/**.
- Disk usage is approximately **23%**, leaving sufficient free space.
- Inode utilization is low across all mounted filesystems.
- Temporary filesystems (`tmpfs`) are mounted and operating normally.

---

## Conclusion

The storage health assessment indicates that the Linux system is operating normally. Disk space usage is within acceptable limits, inode utilization is low, and all required filesystems are properly mounted and accessible.
