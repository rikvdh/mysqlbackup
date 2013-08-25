mysqlbackup
===========

Small bash-script to backup all MySQL databases to file.

You can configure whether to compress them with gzip (default is no compression). Change the GZIP variable at the top to "gzip -c",
setting this variable to "cat" changes the compression method to 'no compression'

Fill in the root-password in the credentials file to enable the script to export the databases.
All databases are exported to seperate files, (.sql or .sql.gz depending on the compression method).

Excluding databases from export
-------------------------------

Just fill in the EXCLUDED variable in the script, separate multiple databases with a space.
