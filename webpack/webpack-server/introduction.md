# сервер

The webpack-dev-server is a little Node.js Express server, which uses the webpack-dev-middleware 
to serve a webpack bundle. It also has a little runtime which is connected to the server via Sock.js. 

Let’s say you have the following config file (webpack.config.js):
```
var path = require("path");
module.exports = {
  entry: {
    app: ["./app/main.js"]
  },
  output: {
    path: path.resolve(__dirname, "build"),
    publicPath: "/assets/",
    filename: "bundle.js"
  }
};
```
