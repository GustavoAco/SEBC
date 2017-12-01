# repo configuration
<code>
wget https://dev.mysql.com/get/mysql57-community-release-el7-11.noarch.rpm
yum install ./mysql57-community-release-el7-11.noarch.rpm
yum install mysql-server
</code>
# install client and jdbc 
<code>
yum install mysql
wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-5.1.44.tar.gz
tar zxvf mysql-connector-java-5.1.44.tar.gz
mkdir /usr/share/java
cp mysql-connector-java-5.1.44/mysql-connector-java-5.1.44-bin.jar /usr/share/java/mysql-connector-java.jar
</code>

#start Mysql and create bds

systemctl start mysqld
mysql -u root -p
mysql>create database scm DEFAULT CHARACTER SET utf8;
mysql>create database rman DEFAULT CHARACTER SET utf8;
mysql>create database hive DEFAULT CHARACTER SET utf8;
mysql>create database hue DEFAULT CHARACTER SET utf8;
mysql>create database oozie DEFAULT CHARACTER SET utf8;



