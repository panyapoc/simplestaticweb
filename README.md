# SimpleStaticWeb

for WebServer Demo

1. Launch EC2: Amazon Linux 2 AMI
2. Select t2.micro
3. User data
```
git clone https://github.com/panyapoc/simplestaticweb.git
cd simplestaticweb
python -m SimpleHTTPServer 80
```
4. SG open port 80
