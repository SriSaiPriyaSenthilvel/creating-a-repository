# EX01 - Creating-a-repository

## AIM:
The aim is to create a repository for Red Hat Enterprise Linux 9.0 (RHEL 9.0) containing the AppStream and BaseOS packages for the x86_64 architecture.

## PROCEDURE:
1.Accessing the Server: Log in to the server where you want to create the repository.

2.Create the repository packages.

3.Copying Packages: Copy the AppStream and BaseOS packages from the RHEL 8.0 DVD to the respective directories on your server.

4.Set up the HTTP Server.

5.Generate the repsitory MetaData.

6.Test the repository by accessing it through a web browser or using ‘yum’ on a client machine configured to use this repository.

## PROGRAM / COMMANDS:
```
Developed by:Sri Sai Priya S
Register Number:212222240103
```
```
mkdir -p /var/www/html/content/rhel8.0/x86_64/dvd/AppStream
mkdir -p /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS

cp -r /path/to/rhel8.0/x86_64/dvd/AppStream/* /var/www/html/content/rhel8.0/x86_64/dvd/AppStream/
cp -r /path/to/rhel8.0/x86_64/dvd/BaseOS/* /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS/

createrepo /var/www/html/content/rhel8.0/x86_64/dvd/AppStream/
createrepo /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS/

mkdir -p /var/www/html/content/rhel8.0/x86_64/dvd/AppStream
mkdir -p /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS

cp -r /path/to/rhel8.0/x86_64/dvd/AppStream/* /var/www/html/content/rhel8.0/x86_64/dvd/AppStream/
cp -r /path/to/rhel8.0/x86_64/dvd/BaseOS/* /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS/

createrepo /var/www/html/content/rhel8.0/x86_64/dvd/AppStream/
createrepo /var/www/html/content/rhel8.0/x86_64/dvd/BaseOS/
```
## OUTPUT:
![image](https://github.com/SriSaiPriyaSenthilvel/creating-a-repository/assets/119475702/87d9b957-6302-4b98-b687-0c5e8968bb86)

# RESULT:
The repository is been created successfully containing the AppStream and BaseOS packages for RHEL 9.0 on the server.
