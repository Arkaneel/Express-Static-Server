## Express Static Server 

<p>Hello Everyone Im Arkaneel Roy and I'll show you how to build a staticwebserver in Node.js and Express</p>

### How To Install This Server
<pre><code>git clone https://github.com/Arkaneel/Express-Static-Server</code></pre>
<pre><code>cd express-static-server</code></pre>
<pre><code>npm install --no-bin-links</code></pre>
<pre><code>npm run dev</code></pre>
 
* Place All Your Files In The public Directory
___

Made With ♥️ and Code By Arkaneel Roy

___

# Steps To Make It By YourSelf:

<pre><code>mkdir static-web-server</code></pre>
<pre><code>cd static-web-server</code></pre>
<pre><code>npm init -y</code></pre>
* Add The Following Code Given Bellow In Package.json
<pre><code>"scripts": {
    "dev": "node server.js"
  },</code></pre>

Now Install Express
<pre><code>npm i express --no-bin-links</code></pre>
Make a File Name <pre><code>server.js</code></pre>
Add The Following Code In server.js
<pre><code>// Define the requirements
const express = require('express');
const path = require('path');
const app = express();

// Define the port the web server will listen to
app.set('port', 8080);

// Using Express to serve the static assets
app.use(express.static(path.join(__dirname, './public')));

// Start the server 
const server = app.listen(app.get('port'), function() {
	console.log('The server is running on: ' + app.get('port'));
	console.log('> http://localhost:8080');
});</code></pre>

Made a Directory Named public and add a index.html


Run The Server Command
<pre><code>npm run dev</code></pre>

Et voilà You've Made Your Web Server

YOU CAN SEE IT IN THE BROWSER WITH URL:

[http://localhost:8080](http://localhost:8080)
