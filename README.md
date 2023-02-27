# argv.helper
Library for coding shell scripts

The helper updates its content and allows you to exec functions as command line arguments

For example:

**./argv.helper --fun2 world!**

`Hello world!`

# http.helper
Library for coding shell scripts

The helper uses **socat** and allows you to exec functions over http

For example:

Server **./http.helper --http_server**

`Serving HTTP on 127.0.0.1 port 8888 (http://127.0.0.1:8888/) ...`

Client **curl http://localhost:8888/test_echo/Hello%20World%21**

`Hello World!`
