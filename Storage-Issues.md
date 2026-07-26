# Storage Troubleshooting Guide

## No Space Left on Device

### Problem

The system reports that there is no available storage space.

### Solution

Check disk usage:

```bash
df -h
```

Delete unnecessary files and packages.

---

## Cannot Access Internal Storage in Termux

### Problem

Termux cannot access shared storage.

### Solution

Run:

```bash
termux-setup-storage
```

Allow storage permissions when prompted.

---

## Large Files Consuming Storage

### Problem

Storage is full due to large files.

### Solution

Find large files:

```bash
du -sh * | sort -h
```

Remove files that are no longer needed.

---

## Downloads Folder Is Too Large

### Problem

Downloaded files consume excessive storage.

### Solution

Review and delete unnecessary files from the Downloads folder.

---

## Unable to Create New Files

### Problem

The system cannot create new files.

### Solution

Check available storage:

```bash
df -h
```

Free up space if necessary.

---

## Package Installation Fails Due to Storage

### Problem

Packages cannot be installed because of insufficient storage.

### Solution

Remove unused packages:

```bash
pkg autoclean
```

Check storage again:

```bash
df -h
```

---

## Storage Permission Denied

### Problem

Applications cannot access storage.

### Solution

Verify storage permissions in Android settings and rerun:

```bash
termux-setup-storage
```

---

## Check Directory Size

### Problem

Need to identify folders using the most storage.

### Solution

Use:

```bash
du -sh *
```

---

## Clean Package Cache

### Problem

Package cache consumes storage.

### Solution

Run:

```bash
pkg autoclean
```

---

## Storage Best Practices

- Remove unnecessary files regularly
- Clear package cache
- Monitor disk usage
- Keep backups of important files
- Organize files into folders
