# SSH Troubleshooting Guide

## SSH Command Not Found

### Problem

The SSH command is unavailable.

### Solution

Install OpenSSH:

```bash
pkg install openssh
```

Verify installation:

```bash
ssh -V
```

---

## SSH Connection Refused

### Problem

Unable to connect to the SSH server.

### Solution

Make sure the SSH service is running:

```bash
sshd
```

Check listening ports:

```bash
netstat -tuln
```

---

## Connection Timed Out

### Problem

SSH connection hangs and eventually times out.

### Solution

Check network connectivity:

```bash
ping <server-ip>
```

Verify firewall and network settings.

---

## Permission Denied (Public Key)

### Problem

SSH key authentication fails.

### Solution

Verify the correct public key is installed on the server.

Check key files:

```bash
ls ~/.ssh
```

---

## Host Key Verification Failed

### Problem

SSH reports a host key mismatch.

### Solution

Remove the old key:

```bash
ssh-keygen -R <hostname>
```

Reconnect:

```bash
ssh user@hostname
```

---

## Cannot Resolve Hostname

### Problem

SSH cannot find the server name.

### Solution

Check DNS resolution:

```bash
ping hostname
```

Or use the server IP address directly.

---

## Check SSH Server Status

### Problem

Need to verify that SSH is running.

### Solution

Use:

```bash
ps aux | grep sshd
```

---

## Generate SSH Key

### Problem

No SSH key exists.

### Solution

Generate a new key:

```bash
ssh-keygen -t rsa -b 4096
```

Or:

```bash
ssh-keygen -t ed25519
```

---

## Copy SSH Key to Server

### Problem

Need to enable key-based authentication.

### Solution

Display public key:

```bash
cat ~/.ssh/id_rsa.pub
```

Copy the output to the server's:

```text
~/.ssh/authorized_keys
```

---

## SSH Best Practices

- Use key-based authentication
- Keep private keys secure
- Disable unused accounts
- Verify server fingerprints
- Use strong passwords when keys are unavailable
