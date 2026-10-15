# Security Audit Report

## The Principle of Least Privilege (PoLP)
The Principle of Least Privilege means that every user, application, or
process should receive only the access it truly needs to perform its task,
and no extra permissions beyond that. This matters for cloud accounts
because an over-privileged account that gets compromised hands the attacker
a lot of power. When an account is tightly scoped, the attacker can only
reach what that account was allowed to touch, so one breach doesn't turn
into a takeover of the entire system.

## Attack Surface
The attack surface of a virtual machine is the sum of all the places an
unauthorized person could try to break in. Open ports, running services,
installed software, and user accounts all add to it. A smaller attack
surface leaves attackers fewer chances to find a weakness, which is why
hardening a server involves turning off or removing everything that isn't
absolutely required.

## Default Deny Policy
A default deny policy blocks all traffic unless it has been specifically
approved, and this is safer than trying to blacklist known attackers one at
a time. No one can anticipate every malicious IP address or attack method
ahead of time. By treating all traffic as untrusted until it is explicitly
permitted, the firewall shuts out unknown and future threats too, instead
of reacting to each one after it has already happened.
