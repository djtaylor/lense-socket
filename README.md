### Lense API Socket.IO Proxy

Socket.IO proxy for making requests to the Lense API engine.

# Node.js Binary

You should create a symlink to the nodejs binary using the following command:

```sh
$ sudo ln -s /usr/bin/nodejs /usr/bin/node
```

# NPM Memory Issues

If you are running on a host with limited memory, and are encountering segfault errors when using NPM, you can try the following workaround:

```sh
$ npm config set jobs 1
```

# Node.js Modules

The Socket.IO proxy depends on certain modules available from NPM, and looks for them in a specific location. You should install the required modules using the following command:

```sh
$ sudo npm install --prefix /usr/share/lense/socket socket.io winston
```