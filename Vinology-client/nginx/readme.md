Master process: Read and evaluate configuration and mantain worker processes

Worker process: They process the requests

By default, the configuration file is named nginx.conf and placed in the directory /usr/local/nginx/conf, /etc/nginx

Starting, Stopping, and Reloading Configuration
To start nginx, run the executable file. Once nginx is started, it can be controlled by invoking the executable with the -s parameter. Use the following syntax:
``
$ nginx -s signal
``

Where signal may be one of the following:


stop — fast shutdown
quit — graceful shutdown
reload — reloading the configuration file
reopen — reopening the log files

example:
``
nginx -s quit
``

Proxy server

server {
    location / {
        proxy_pass http://localhost:3002;
    }

        location {
        root http://localhost:3000;
    }
}


/etc/nginx

copy folder from contaner 

sudo docker cp nginx-base:/etc/nginx/conf.d/default.conf /default.conf