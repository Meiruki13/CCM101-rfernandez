# Reflection

A host-based firewall keeps a server safe even when the outer network
defenses fail, because it applies protection on the server itself rather
than only at the network's edge. If an attacker slips past a router or
network firewall and reaches the machine directly, UFW still checks every
incoming connection against its own rules and rejects whatever hasn't been
specifically permitted. The server never assumes the network around it can
be trusted.

Controlling open ports is essential for shrinking a server's attack
surface, since each open port is another door an attacker can try. If a
service behind a port has a known vulnerability, leaving that port open
practically invites an attack. Closing every port the server doesn't need
removes whole categories of threats before anyone even attempts them.

Exposing a database port such as 3306 to the public internet is risky
because anyone online can try to connect straight to the database and skip
the application layer completely. Databases usually store the most
sensitive information in a system, so one that faces the internet can be
hit with brute-force logins or known exploits and be compromised without
the attacker ever going near the web application in front of it.

This mission changed how I think about server security. Before setting up
UFW myself, I didn't realize that a freshly deployed server is already
vulnerable the instant it goes online, not only after months of neglect.
One small slip, like enabling the firewall before allowing SSH, can lock an
administrator out just as easily as a sloppy rule can leave the server wide
open.

My GitHub portfolio now holds eight finished missions, each one building
on the previous, starting with basic Linux navigation in Mission 1 and
moving through infrastructure as code and observability to security
hardening here. Viewed as a whole, the repository no longer feels like a
pile of separate assignments. It reads as a steady progression toward real
cloud engineering practice.
