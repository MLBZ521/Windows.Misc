Windows.Misc
======

In this repository are various scripts that I have written that are random or possibly used for proprietary/LOB software.


#### EagleSoft ####

A client I supported used Patterson EagleSoft which is a Dental Clinic software package.  I inherited an 'interesting' setup where they copied the 'data set' from one 'server' to external USB media and then to another 'server.'  Their previous IT support wrote a simple script that copied the entire collection of files every time.  I would regularly receive calls because the external drive was full, along with the staff not following the proper steps of shutting down the Patterson services, which lead to incomplete copies.  I wrote two scripts (a Backup and a Restore) that handled the entire process for them and used `rsync` to only copy the *CHANGED* files which resulted is much faster 'backups' and 'restores' from their end.
