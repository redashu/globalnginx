# Nginx day2

## nginx as reverse proxy 

<img src="rev.png">

## New nginx server as reverse proxy 

```
[root@vm111 conf.d]# cat  default.conf 
server {
    listen       80;
    server_name  localhost;

    #charset koi8-r;
    #access_log  /var/log/nginx/host.access.log  main;

    location / {
        #root   /usr/share/nginx/html;
        #index  index.html index.htm;
	proxy_pass  http://40.122.25.60;
    }


```

## Nginx as Loadbalancer 

### using Round-Robin algo 

<img src="rr.png">

### least-connected & IP-hash 

<img src="algolb.png">

