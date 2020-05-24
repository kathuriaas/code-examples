# http server in nodejs

## Following are steps to create a very simple http server. we need http module, which is part of default installation of nodejs

## nodejs should be already installed. If not, follow the [installation steps](./install_nodejs.md)

Create a file *app.js* at any location on your computer and add below code to it:

```nodejs
var http = require('http');

httpServer = http.createServer(function(req,res){
    res.writeHead(200,{'Content-Type':'text/plain'});
    res.end('Hello World');
    });

httpServer.listen(8080);
```

Above code will create an http server.

Now, start your nodejs server using following command:-

```nodejs
node app.js
```

Now, open link <http://localhost:8080/> in your favourite browser and you should see "Hello World" on the page.