### Initial Setup

1. Download splunk install image and MD5sum file (you will need a splunk.com user for it)
```bash
wget -O splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb "https://download.splunk.com/products/splunk/releases/9.2.1/linux/splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb"
```

2. Check MD5 hash
```bash
$ echo "6cf3e47174f54f826b15ebc1ab8616b7 splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb" | md5sum -c
splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb: OK
```

3. Install Splunk
```bash
dpkg -i splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb
```

4. check the installation
```bash
$ dpkg --status splunk
Package: splunk
Status: install ok installed
Maintainer: Splunk Inc. <info@splunk.com>
Architecture: amd64
Version: 9.2.1+78803f08aabb
Description: Splunk The platform for machine data.
```

5. Create a user-seed file with credentials
```bash
$vim /opt/splunk/etc/system/local/user-seed.conf

[user_info]
USERNAME = admin
PASSWORD = $uperSplunk77
```
6. Enable auto-boot of Splunk and accept the license
```bash
$/opt/splunk/bin/splunk enable boot-start --accept-license
Init script installed at /etc/init.d/splunk.
Init script is configured to run at boot.
```

7a. Start Splunk
```bash
/opt/splunk/bin/splunk start
```

7b alternative way to start Splunk
```bash
systemctl start Splunkd
```



10. start splunk, accept EULA, create a usernam (e.g. admin) and password
```bash
/opt/splunk/bin/splunk start
```

