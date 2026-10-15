# Automation Research

## Bash Script
A Bash script is a text file made up of Linux commands that the shell runs
one after another from the first line to the last, just as though someone
were typing them by hand. The `#!/bin/bash` line at the very top is known
as the shebang, and it tells the operating system which interpreter, here
Bash, should read and execute the rest of the file.

## Variables
Programmers use variables such as `$BACKUP_DIR` rather than writing out a
full folder path each time, because it keeps scripts easier to maintain and
cuts down on mistakes. When the backup location changes, only the one
assignment at the top of the script needs updating, instead of searching
through the whole file for every command that mentions that path.

## Cron Job
A cron job is a task scheduled with Linux's built-in `cron` service, which
runs a chosen script or command on its own at a set time, date, or
interval without anyone having to start it. It is essential in cloud
operations because important routine work, such as backups, shouldn't rely
on someone remembering to do it every day. Cron takes the human out of the
loop completely.
