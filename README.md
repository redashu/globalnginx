# Web servers 

<img src="web.png">

## tomcat & IIS 

<img src="iistom.png">

## httpd | tomcat | nginx 

<img src="webs.png">

## some official URLs 

[URL official] ('https://www.nginx.com/')

## Docs & GUide 

[docs] ('https://nginx.org/en/docs/')

## Nginx offerings 

<img src="ngoffer.png">

## Nginx installation 

<img src="nginstall.png">


## check OS details

<img src="oscheck.png">

## Installation steps 

### check and update rhel if it is having gcc / python based upgrades 

```
yum update -y

```

## install URL 

[install nginx] ('https://nginx.org/en/linux_packages.html')

## creating nginx online repo 

```
[root@ashunginxvm1 ~]# cd  /etc/yum.repos.d/
[root@ashunginxvm1 yum.repos.d]# ls
redhat.repo  rh-cloud-eus.repo
[root@ashunginxvm1 yum.repos.d]# vim  nginx.repo 
[root@ashunginxvm1 yum.repos.d]# 

```

## content of nginx.repo

```


[root@ashunginxvm1 ~]# cat  /etc/yum.repos.d/n.repo 
[nginx]
name=nginx repo
baseurl=https://nginx.org/packages/rhel/7/$basearch/
gpgcheck=0
enabled=1
[root@ashunginxvm1 yum.repos.d]# 

```


