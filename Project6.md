# Steps for Web Solution With WordPress
* Launched 2 RedHat servers on the AWS console in the same availability zone
* Opened the security groups to all
* Named servers Web server and Database server
* On the Web server, created three 10G volumes
* Connected to the instance
* Attached all three volumes to the Web server instance
* Confirmed block devices attached to the server by running the lsblk command on the terminal
* Configured all 3 disks and created a partition each on them
* Installed lvm2
* Created Physical volumes on all 3 devices
* Created a volume group named webdata-vg for the 3 devices
* Created 2 locgical volumes of 14G each named app-lv and log-lv
* Created ext4 file systems on both logical volumes
* Created a mount point for the devices
* Mounted app-lv on www/var/html
* Copied entire data from /var/log in to /home/recovery/logs/
* Mounted log-lv unto /var/log
* Restored the var/log folder by copying back the data
* Configured fstab
* Reloaded the daemon
* Repeat all steps from line 5 for the Database server
* Created a 20G logical volume named db-lv, created the ext4 file system and mounted it unto the /db directory
* Configured the fstab file for the db
* Reloaded the daemon
* Installed WordPress on the WebServer
* Installed the latest version of PHP and it's dependencies
* Restarted httpd
* Created a WordPress directory
* Changed directory into WordPress
* Copied the sample.php file into the config.php file
* Copied the contents of wordpress into /var/www/html
* Changed directory to /var/www/html
* Installed mysql on the DB server
* Created a wordpress database and created a wordpress user with a password
* <img width="1646" alt="PROJECT 6 WORDPRESS DB" src="https://user-images.githubusercontent.com/86001367/123792749-e0252b80-d8d8-11eb-95c9-fddfaad213cb.png">
* <img width="1253" alt="PROJECT 6 SQL HOST" src="https://user-images.githubusercontent.com/86001367/123792873-02b74480-d8d9-11eb-991e-4adbe299dbd3.png">
* <img width="1665" alt="PROJECT 6 WORDPRESS SITE" src="https://user-images.githubusercontent.com/86001367/123792931-1793d800-d8d9-11eb-96af-6f3041036eb7.png">
* <img width="1664" alt="PROJECT 6 WEBSEVER TO DB SERVER CONNECTION" src="https://user-images.githubusercontent.com/86001367/123792995-28dce480-d8d9-11eb-90a4-27bc423ab94d.png">




* Granted and flushed privileges
