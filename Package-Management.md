# Package Management Troubleshooting

## Package Not Found

### Problem

The package manager cannot find the requested package.

### Solution

Update package lists:

```bash
pkg update
```

Or:

```bash
apt update
```

Search for the package:

```bash
pkg search <package-name>
```

---

## Failed to Fetch Packages

### Problem

Unable to download package information.

### Solution

Check internet connectivity:

```bash
ping google.com
```

Update repositories:

```bash
pkg update
```

---

## Broken Dependencies

### Problem

Package installation fails because of dependency issues.

### Solution

Upgrade installed packages:

```bash
pkg upgrade
```

Then try again.

---

## Repository Errors

### Problem

Repository metadata is outdated or corrupted.

### Solution

Refresh package information:

```bash
pkg update
```

---

## Unable to Install Package

### Problem

Installation process stops with errors.

### Solution

Check available storage:

```bash
df -h
```

Update package lists:

```bash
pkg update
pkg upgrade
```

---

## Package Already Installed

### Problem

The package manager reports that the package already exists.

### Solution

Verify installation:

```bash
pkg list-installed
```

---

## Outdated Packages

### Problem

Installed packages are old.

### Solution

Upgrade all packages:

```bash
pkg upgrade
```

---

## Remove Unused Packages

### Problem

Unnecessary packages consume storage.

### Solution

Remove package:

```bash
pkg uninstall <package-name>
```

Example:

```bash
pkg uninstall nano
```

---

## Check Installed Packages

### Problem

Need to view installed packages.

### Solution

Use:

```bash
pkg list-installed
```

---

## Package Management Best Practices

- Run updates regularly
- Remove unused packages
- Verify internet connectivity before updating
- Keep package repositories current
- Review package names before installation
