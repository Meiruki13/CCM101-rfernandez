# Firewall Configuration

## Allow SSH
```bash
sudo ufw allow ssh
```

## Default Deny Policy
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## Enable Firewall
```bash
sudo ufw enable
```

### Output
```
Rules updated
Rules updated (v6)
Default incoming policy changed to 'deny'
(be sure to update your rules accordingly)
Default outgoing policy changed to 'allow'
(be sure to update your rules accordingly)
Firewall is active and enabled on system startup
```

## Verify Firewall Status
```bash
sudo ufw status verbose
```

### Output
```
Status: active
Logging: on (low)
Default: deny (incoming), allow (outgoing), deny (routed)
New profiles: skip

To                         Action      From
--                         ------      ----
22/tcp                     ALLOW IN    Anywhere
22/tcp (v6)                ALLOW IN    Anywhere (v6)
```

## Allow Port 8080 (Web Application)
```bash
sudo ufw allow 8080/tcp
```

## What happens if `ufw enable` runs before `ufw allow ssh`?
If `sudo ufw enable` is run before SSH is allowed, the firewall immediately blocks all incoming traffic, including the SSH session that is currently open. The administrator would be locked out of the server and could only get back in through the cloud provider's emergency console.
