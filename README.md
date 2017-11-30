# hostloc auto-view tool

A PHP script to automatic get 20 points from hostloc with crontab.

##HOW TO USE
1. You need a vps with PHP envirnoment, PHP5.0 to PHP7.1 are all suitable.<br>
2. Download this program to any usable folder, such as /var/www/html/. Change the USERNAME and PASSWORD to your username and password.<br>
Actually, you can run it by "PHP sign.php", but it is not auto-run.<br>
3. If you want to auto-run this rogram, crontab should have been installed in your vps. If the vps did not have crontab, for Debian(Ubuntu, deepin...):<br>
```
sudo apt-get install crontab -y
```
for CentOS(RedHat...):<br>
```
sudo yum install crontab -y
```
And use set a auto-run rask.<br>
```
30 21 * * * /usr/bin/php -f /var/www/html/sign.php >> sign.log
```
It means this PHP script will auto-run at 21:30 everyday, and it will write a feedback into sign.log.<br>
<br>
<br>
The Script is from hostloc http://www.hostloc.com/thread-306269-1-1.html.
