# Socket.IO Benchmark

## Install Dependencies on Ubuntu

```
sudo apt-get install python python-dev python-pip maven
sudo pip install websocket
```

## Clone and initialize this repo

```
git clone https://github.com/drewww/socket.io-benchmarking.git
cd socket.io-benchmarking
sudo npm install
cd client
mvn install
cd ..
```

## Start the server on port 94104

```
node server.js -p 94104
```

## Start the client

```
#localhost port 94104; 2 connections; 20 messages per second
python client.py localhost -p 94104 -c 2 -C 20
```
