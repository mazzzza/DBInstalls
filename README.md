# DBInstalls
## install / uninstall DBs

* ref: <https://qiita.com/egplnt/items/99fdf456b67e9726ee0d>

### delete current MySQL resources:

* ref: <https://community.jaspersoft.com/wiki/uninstall-mysql-mac-os-x>

* To uninstall MySQL and completely remove it (including all databases) from your Mac do the following:

Open a terminal window

Use mysqldump to backup your databases to text files!

Stop the database server

`sudo rm /usr/local/mysql`
`sudo rm -rf /usr/local/mysql*`
`sudo rm -rf /Library/StartupItems/MySQLCOM`
`sudo rm -rf /Library/PreferencePanes/My*`
edit `/etc/hostconfig` and remove the line `MYSQLCOM=-YES-`
`rm -rf ~/Library/PreferencePanes/My*`
`sudo rm -rf /Library/Receipts/mysql*`
`sudo rm -rf /Library/Receipts/MySQL*`
`sudo rm -rf /private/var/db/receipts/*mysql*`

The last three lines are particularly important as otherwise, you can't install an older version of MySQL even though you think that you've completely deleted the newer version!

### how to use "find" command:

c.f: find recursively from current directory for name starting with "pro":
`find . -name pro\*`
