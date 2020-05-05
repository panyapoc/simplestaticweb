# SimpleStaticWeb

## S3 Static Website

1. Make S3 bucket to host the website

``` bin/bash
aws s3 mb s3://mybucket --region ap-southeast-1
```

2. Copy the asset to the bucket

``` bin/bash
aws s3 cp ./dist s3://mybucket/ --recursive
```

1. Create CF

``` bin/bash
aws
```


## Use in WebServer

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

4. SG open port 80
