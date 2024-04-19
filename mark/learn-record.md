nginx
根目录下的conf是配置文件，真正起到作用的。html中的conf是复制进去的用来记录修改的过程。
因为改成了单台服务器，所以需要把backend注释掉，并且upstream也注释掉
proxy_pass http://127.0.0.1:8081;
proxy_pass http://backend;
