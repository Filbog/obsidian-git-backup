11-01-2025

1. set up a "safe tunnel" to fly.io
2. Use pg_dump command to export the database
	1. watch out for different postgresql versions installed on your computer! If we want to upgrade our postgresql, brew will choose a 'default' version. And we can have like postgresql@14, postgresql@16... I had to uninstall v14 to make it work. Otherwise I got the "server mismatch" error.



### Hashtags:
#coding #flydotio

### References (source material, similar notes):
some info:
https://community.fly.io/t/exporting-postgres-table-to-local-file/11281 
good tutorial. For Windows, but works for mac too. I got the command from here:
https://community.fly.io/t/backup-and-restore-postgresql-in-fly-io-step-by-step/11455 
Different postgres versions issue:
https://stackoverflow.com/questions/45025382/how-to-update-pg-dump-to-server-version-in-mac-os 