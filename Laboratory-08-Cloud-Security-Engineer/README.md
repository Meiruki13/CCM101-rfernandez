# Laboratory Activity 8: Mission 8 – The Cloud Security Engineer

## Mission Overview
This lab puts defense-in-depth into practice by hardening a live server
with a host-based firewall. It involved launching a publicly reachable web
application, reviewing which ports were open, and setting up UFW with a
Default Deny policy so that every connection is blocked except the ones
the application genuinely requires.

## Objectives
- Explain what an attack surface is and how the Principle of Least Privilege reduces risk
- Carry out a basic security audit of the server's active network ports
- Set up UFW with a Default Deny policy
- Apply fine-grained port rules to allow only SSH and web (HTTP) traffic

## Commands Executed
- `docker run -d --name secure-web-app -p 8080:80 nginx` — launched the publicly exposed web app
- `sudo ufw allow ssh` — permitted SSH first, before turning the firewall on
- `sudo ufw default deny incoming` / `sudo ufw default allow outgoing` — established the Default Deny policy
- `sudo ufw enable` — turned the firewall on
- `sudo ufw status verbose` — checked the active rules and default policies
- `sudo ufw allow 8080/tcp` — opened only the port the web app depends on
- `sudo ufw status numbered` — confirmed the new rule was in place

## Skills Learned
- Setting up a host-based firewall using a Default Deny policy
- Recognizing why rule order matters, since SSH must be allowed before the firewall is enabled
- Managing individual ports to keep a server's attack surface as small as possible
- Writing clear security documentation that other engineers can follow
