# Ubuntu Node

1.
```
sudo apt-get update
sudo apt-get install nodejs
sudo apt-get install git
sudo apt-get install npm
```

2.
This will resolve the naming conflict.
```
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

3.
```
npm install -g express-generator
```

4.
```
express
```

5.
pm2
```
pm2 delete server.js
```

Sources:

[Installing Node Express on Ubuntu]
[Tiny Node "Hello World" on Ubuntu]

[Installing Node Express on Ubuntu]: http://iws.io/hosting-a-nodejs-express-application-on-amazon-web-services-ec2/

[Tiny Node "Hello World" on Ubuntu]: https://www.digitalocean.com/community/tutorials/how-to-set-up-a-node-js-application-for-production-on-ubuntu-14-04