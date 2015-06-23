# xen_migrate

In order to use this script you must first run the following command on your .xva file.

    tar -xvf mybackup.xva

This will create a folder called Ref:XXX the X is a random number that is generated via XenServer 
during the backup process. Once this completes, note it will take a significant amount of time
especially if your backup is huge and your drive is slow. Needs patience. 

Once it finishes you will then run this command.

    python xen_migrate.py --convert=/home/<username>/Ref:XXX <nameofimagefile>.img

This will create a .img file for you to use with your xen-hypervisor. Happy converting!
