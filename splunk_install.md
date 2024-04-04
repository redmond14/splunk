### Initial Setup

1. Download splunk install image (you will need a splunk.com user for it)
```bash
wget -O splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb "https://download.splunk.com/products/splunk/releases/9.2.1/linux/splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb"
```

2. Check MD5 hash
```bash
$ echo "6cf3e47174f54f826b15ebc1ab8616b7 splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb" | md5sum -c
splunk-9.2.1-78803f08aabb-linux-2.6-amd64.deb: OK
```
