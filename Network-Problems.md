# Common Network Problems and Solutions

## No Internet Connection

### Problem

Device cannot access the internet.

### Solution

Check connectivity:

```bash
ping 8.8.8.8
```

Check Wi-Fi or mobile data connection.

---

## DNS Resolution Failed

### Problem

Websites cannot be reached by name.

### Solution

Test DNS:

```bash
nslookup google.com
```

Try using a different DNS server.

---

## High Latency

### Problem

Slow response time and lag.

### Solution

Check network quality:

```bash
ping google.com
```

Look for high ping times or packet loss.

---

## Cannot Reach Host

### Problem

Unable to communicate with another device.

### Solution

Verify IP address and network configuration.

```bash
ping <ip-address>
```

---

## SSH Connection Timeout

### Problem

SSH connection cannot be established.

### Solution

Verify the SSH service is running and the correct port is open.

```bash
sshd
```

---

## Network Interface Not Working

### Problem

Network adapter is not responding.

### Solution

Check interface status:

```bash
ip addr
```

---

## Packet Loss

### Problem

Intermittent connectivity issues.

### Solution

Run a continuous ping test:

```bash
ping google.com
```

Investigate unstable connections or weak signals.

---

## Website Not Loading

### Problem

Browser cannot open websites.

### Solution

Check internet access and DNS settings.

```bash
ping google.com
```

---

## Slow Downloads

### Problem

Downloads are taking too long.

### Solution

Test internet speed and switch networks if necessary.

---

## IP Address Conflict

### Problem

Two devices have the same IP address.

### Solution

Renew IP configuration or assign a different IP address.
