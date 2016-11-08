
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