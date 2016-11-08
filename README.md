
# node-server

## Install node
```shell
curl -sL https://deb.nodesource.com/setup_7.x | sudo -E bash -
apt-get install -y nodejs
```

## Install the app
```shell
# Install Forever
npm install -g forever
npm install -g forever-service

# Install the app as a service
forever-service install -s index.js node-server

# Start the service
service node-server start
```

## Check the status of te APP

### From a terminal
```shell
# Get the status
forever list

# tail the logs
tail -f /var/log/node-server.log
```

### From a web browser
go to ```http://<ip>:3000/```, Hello world should be displayed.
