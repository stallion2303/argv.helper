Librares for coding shell scripts

# argv.helper

It is required to describe the functions as

```
def fun << 'EOF'
    echo 'exec fun'
EOF
```

The helper updates its content and allows you to exec functions as command line arguments

For example:

**./argv.helper --fun2 world!**

`Hello world!`

# http.helper

The helper uses **socat** and allows you to exec functions over http

For example:

Server **./http.helper --http_server**

`Serving HTTP on 127.0.0.1 port 8888 (http://127.0.0.1:8888/) ...`

Client **curl http://localhost:8888/test_echo/Hello%20World%21**

`Hello World!`

# argv.helper.legacy

Just add it to your script and exec functions as command line arguments

For example:

**./argv.helper.legacy --fun2**

`fun2`

## Tested Environments

docker [ apline:latest | debian:latest | ubuntu:latest | rockylinux:latest ]
 
