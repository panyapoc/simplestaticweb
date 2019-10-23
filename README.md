# SimpleStaticWeb

for WebServer Demo

1. Launch EC2: Amazon Linux 2 AMI
2. Select t2.micro
3. User data

``` bash
#!/bin/bash
sudo yum install git
sudo yum install tmux
tmux
git clone https://github.com/panyapoc/simplestaticweb.git
cd simplestaticweb/
sudo python -m SimpleHTTPServer 80
```

1. SG open port 80
