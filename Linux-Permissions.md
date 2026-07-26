# Linux Permissions Troubleshooting

## Permission Denied

### Problem

You receive a "Permission denied" error when trying to run a file.

### Solution

Make the file executable:

```bash
chmod +x filename.sh
```

Run the file:

```bash
./filename.sh
```

---

## Cannot Edit a File

### Problem

You do not have permission to modify a file.

### Solution

Check file permissions:

```bash
ls -l
```

Change permissions if needed:

```bash
chmod 644 filename
```

---

## Script Will Not Execute

### Problem

A shell script exists but will not run.

### Solution

Make it executable:

```bash
chmod +x script.sh
```

---

## Check File Permissions

### Problem

Need to verify current permissions.

### Solution

Use:

```bash
ls -l
```

Example output:

```text
-rwxr-xr-x
```

---

## Change File Permissions

### Problem

Need to grant or remove permissions.

### Solution

Examples:

```bash
chmod 755 script.sh
chmod 644 file.txt
```

---

## Change File Ownership

### Problem

Wrong owner assigned to a file.

### Solution

Use:

```bash
chown username filename
```

Example:

```bash
chown noel notes.txt
```

---

## Read, Write, Execute Explained

### Read (r)

Allows viewing file contents.

### Write (w)

Allows modifying file contents.

### Execute (x)

Allows running a file as a program.

---

## Common Permission Values

| Value | Meaning |
|---------|---------|
| 777 | Full permissions |
| 755 | Owner full access |
| 644 | Read/write for owner |
| 600 | Owner only |

---

## Best Practice

Avoid using:

```bash
chmod 777
```

unless absolutely necessary.

Use the minimum permissions required.
