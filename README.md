# Ansible
FOLDER cron_template:
  FILE marinkoco /Cron Job template declaring reccurence of triggering fileSize.sh script and writting output to a cronLogTest.log
FOLDER CRON_TEST:
  FILE cronFile.txt /ref.- in line 7
  FILE cronLogTest.txt /ref.- in line 3
  FILE fileSize.sh /Bash Script that pull size of a file cronFile.txt which gets written to cronLogTest.txt by cron job ref.- in line 3
FILE copyFolder.yml /Ansible playbook that copies CRON_JOB folderand sets cron job described in line 3
FILE SYM.yml /Ansible playbook that creates sym link using folder masking in path (used when folder in a path changes due to naming convention of the machines)
