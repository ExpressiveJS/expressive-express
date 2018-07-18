# expressive-express
[Expressive.js](https://github.com/bugs181/Expressive.js) protocol plugin for [Express](https://github.com/expressjs/express)

<br>

### Expressive.js CLI Install: ###

    npm install expressive-cli -g
    expressive init myProject
    expressive install express
    expressive start

<br>

### Manual Install: ###

    cd myProject
    npm install expressive --save
    cd /node_modules/expressive
    npm install expressive-express

<br>

### Expressive.js config.js: ###
    {
        protocols: ['express'],
        
        express: {
          port: 8082,
          static: `${require('path').join(__dirname, '../web/static')}`,
          
          // See note on other middlewear options
        }
    }

<br>

### Other middlewear options: ###
This project uses [expressive-middlewear](https://github.com/bugs181/expressive-middleware). <br>
Any options allowed by that framework can be used in the config object as well.
