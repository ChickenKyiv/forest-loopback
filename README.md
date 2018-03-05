# Forest Loopback connector
The official Loopback liana for Forest.

## Installation

1. Run `$ npm install forest-loopback --save`
2. Add the following code to your `server/server.js` file:
```javascript
app.use(require('forest-loopback').init({
  modelsDir: __dirname + '/../common/models',  // The directory where all of your Loopback models are defined.
  secretKey: 'ultrasecretkey', // The secret key given my Forest.
  authKey: 'catsOnKeyboard', // Choose a secret authentication key.
  loopback: require('loopback') // The loopback instance given by require('loopback').
}));
```

# License

[GPL v3](https://github.com/ForestAdmin/forest-loopback/blob/master/LICENSE)
