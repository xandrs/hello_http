# hello_http
Hello world with a webserver in C


## How to build
```gcc -o dummyserv dummy_serv.c```

Or to build a static binary

```gcc -o dummyserv dummy_serv.c```

## How to run
The port argument is optional and when not included the service will default to port 8080

```dummyserv <port>```
=========================

Instruction how to Run next commands on Windows:

vagrant up
vagrant ssh => enter vagrant as password if promped (on Windows)
cd /vagrant

Without next 2 commands will be not able to install gcc. They are requiread on Windows.
sudo apt-get update
sudo apt-get install build-essential

gcc -o dummyserv dummy_serv.c => after running this command dummyserv file will appear inside http_hello folder
./dummyserv 12344 => after running this command you will see in terminal window:
socket created successfully
socket successfully bound to address:12344
server listening for connections

Open http://localhost:12344/ in webbrowser => Should see: hello, world

These lines will appears in the terminal too:
connection accepted
[10.0.2.15:12344] GET HTTP/1.1 /
connection accepted
[10.0.2.15:12344] GET HTTP/1.1 /favicon.ico




