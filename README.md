# hostloc auto-view tool

A PHP script to automatic get 20 points from hostloc with crontab.

#HOW TO USE
1. You need a vps with PHP envirnoment, PHP5.0 to PHP7.1 are all suitable.<br>
2. Download this program to any usable folder, such as /var/www/html/. Change the USERNAME and PASSWORD to your username and password.<br>
Actually, you can run it by input "PHP sign.php", but it is not auto-run.<br>
3. If you want to auto-run this rogram, crontab should have been installed in your vps. If the vps does not have crontab, or Debian(Ubuntu, deepin...):<br>
sudo apt-get install crontab -y<br>
for CentOS(RedHat...):<br>
sudo yum install crontab -y<br>
And use set a auto-run rask.<br>
30 21 * * * /usr/bin/php -f ~/sign.php >> sign.log<br>
For example
