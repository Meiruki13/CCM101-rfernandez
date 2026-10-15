# Reflection

Automation matters a great deal when hundreds of cloud servers are involved,
because manual administration cannot keep up. A job that takes a minute on
one server turns into hours of repetitive, mistake-prone work across a whole
fleet. A script written once runs identically on every machine in an
instant, while a person retyping commands will eventually mistype one or skip
a step.

The danger of automation comes from the same thing that makes it powerful:
scale. If an administrator slips up while updating one server by hand, only
that server is affected. If the same slip is built into a script scheduled
for 1,000 servers, it is carried out perfectly everywhere at once, turning a
small human error into a massive outage in seconds. Knight Capital Group saw
this in 2012 when a flawed automated deployment cost it $460 million in 45
minutes, as our Chapter 9 module notes.

Writing a Bash script felt like conventional, step-by-step programming:
variables and commands running from top to bottom on one machine. The Docker
Compose YAML file from Mission 6 was declarative instead. Rather than listing
instructions, I described the end state I wanted for a multi-container
system, including the images, how they connect, and their environment
variables, and Docker worked out how to get there.

Looking back over my repository from Laboratory 1 to Laboratory 9, my view of
cloud computing has changed from seeing it as a remote place to keep files to
seeing it as a complete discipline. It covers provisioning infrastructure,
deploying containers, managing data, securing a server with a firewall,
monitoring its health, and now automating routine maintenance. Every lab
built directly on what the one before it taught me.

The role I enjoyed most was the Cloud Automation Engineer, because watching a
script I wrote create a backup on its own, then scheduling it with cron so
nobody has to run it, showed me how much repetitive work can be handed to the
system.
