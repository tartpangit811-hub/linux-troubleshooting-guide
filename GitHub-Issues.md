# Common GitHub Issues and Solutions

## Authentication Failed

### Problem

Unable to push changes to GitHub.

### Solution

Check your GitHub credentials and authentication method.

---

## Repository Not Found

### Problem

Git cannot find the repository.

### Solution

Verify the repository URL:

```bash
git remote -v
```

---

## Push Rejected

### Problem

Remote repository contains changes not present locally.

### Solution

Pull first:

```bash
git pull origin main
```

Then push again:

```bash
git push origin main
```

---

## Merge Conflict

### Problem

Git cannot automatically merge changes.

### Solution

Manually edit the conflicting files and commit the resolved version.
