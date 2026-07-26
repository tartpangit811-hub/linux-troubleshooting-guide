# Python Troubleshooting Guide

## Python Command Not Found

### Problem

Python is not installed.

### Solution

Install Python:

```bash
pkg install python
```

Verify installation:

```bash
python --version
```

---

## Pip Command Not Found

### Problem

Pip is unavailable.

### Solution

Check pip installation:

```bash
pip --version
```

Reinstall Python if necessary:

```bash
pkg reinstall python
```

---

## Module Not Found Error

### Problem

Python cannot find a required module.

### Solution

Install the missing package:

```bash
pip install <module-name>
```

Example:

```bash
pip install requests
```

---

## Permission Denied During Installation

### Problem

Pip cannot install packages.

### Solution

Upgrade pip:

```bash
pip install --upgrade pip
```

---

## Python Script Will Not Run

### Problem

Script produces errors or does not execute.

### Solution

Check syntax:

```bash
python script.py
```

Review the error message carefully.

---

## Virtual Environment Not Found

### Problem

Unable to create or activate a virtual environment.

### Solution

Create environment:

```bash
python -m venv myenv
```

Activate:

```bash
source myenv/bin/activate
```

---

## Package Installation Failed

### Problem

Pip cannot download or install packages.

### Solution

Check internet connectivity:

```bash
ping google.com
```

Upgrade pip:

```bash
pip install --upgrade pip
```

---

## Check Installed Packages

### Problem

Need to view installed Python packages.

### Solution

Use:

```bash
pip list
```

---

## Upgrade Installed Packages

### Problem

Packages are outdated.

### Solution

Upgrade package:

```bash
pip install --upgrade package-name
```

Example:

```bash
pip install --upgrade requests
```

---

## Python Best Practices

- Keep Python updated
- Use virtual environments
- Install only trusted packages
- Regularly update dependencies
- Read error messages carefully
