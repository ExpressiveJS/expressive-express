# expressive-express
[Express](https://github.com/expressjs/express) protocol plugin for [Expressive](https://github.com/bugs181/Expressive)

<br>

### Expressive CLI Install: ###

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

### Expressive config.js: ###
    {
        protocols: ['express'],
        
        express: {
          port: 8082,
          statusInResponse: true,
          routeNotFound: '404', // Can be a 404.html page. fs.fileSync('404.html')
          static: `${require('path').join(__dirname, '../web/static')}`,
        }
    }
