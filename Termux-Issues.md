# Common Termux Issues and Solutions

## Storage Permission Error

### Problem

Unable to access internal storage.

### Solution

Run:

```bash
termux-setup-storage
```

Allow storage permission when prompted.

---

## Package Installation Failed

### Problem

Error while installing packages.

### Solution

Update package lists:

```bash
pkg update
pkg upgrade
```

---

## Command Not Found

### Problem

A command is not recognized.

### Solution

Install the required package:

```bash
pkg install <package-name>
```

Example:

```bash
pkg install git
```

---

## Python Not Found

### Problem

Python is not installed.

### Solution

```bash
pkg install python
```

Verify installation:

```bash
python --version
```

---

## Git Not Found

### Problem

Git command is unavailable.

### Solution

```bash
pkg install git
```

Check version:

```bash
git --version
```

---

## SSH Connection Refused

### Problem

Unable to connect via SSH.

### Solution

Start SSH server:

```bash
sshd
```

Check listening port:

```bash
netstat -tuln
```

---

## Slow Package Downloads

### Problem

Package downloads are very slow.

### Solution

Check internet connection and switch to a faster mirror if available.

---

## No Space Left on Device

### Problem

Storage is full.

### Solution

Check storage usage:

```bash
df -h
```

Remove unnecessary files and packages.

---

## Permission Denied

### Problem

Script cannot be executed.

### Solution

Make it executable:

```bash
chmod +x script.sh
```

Run:

```bash
./script.sh
```

---

## Repository Errors

### Problem

Repository metadata is outdated.

### Solution

Refresh repositories:

```bash
pkg update
```
