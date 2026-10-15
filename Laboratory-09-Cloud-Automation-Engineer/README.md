# Laboratory Activity 9: Mission 9 – The Cloud Automation Engineer

## Mission Overview
This lab removes human error from a repetitive operational task. It involved
writing a Bash script that compresses and backs up a client's application
data on its own, then using the Linux cron scheduler to run that script
every night at 2:00 AM so that nobody has to start it manually.

## Objectives
- Learn the basic syntax of a Bash shell script, including variables and simple commands
- Use the nano text editor to write and save a script that can be executed
- Change Linux file permissions with chmod
- Understand how task scheduling works and how a crontab entry is written
- Document automation code and cron job settings in Markdown

## Commands Executed
- `mkdir app-data` / `echo "..." > app-data/data.txt` — set up sample client data to back up
- `nano backup.sh` — wrote the automated backup script
- `chmod +x backup.sh` — gave the script permission to execute
- `./backup.sh` — ran the script and generated a compressed `.tar.gz` backup
- `crontab -e` — added the cron entry `0 2 * * * /root/backup.sh`
- `crontab -l` — checked that the schedule was installed correctly

## Skills Learned
- Writing a Bash shell script and running it from the terminal
- Controlling Linux file permissions with chmod
- Scheduling recurring tasks to run automatically with cron
- Documenting automation code and scheduling syntax so other engineers can follow it
