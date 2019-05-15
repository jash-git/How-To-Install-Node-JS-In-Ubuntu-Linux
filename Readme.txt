Ubuntu 安裝/測試 nodejs [How To Install Node JS In Ubuntu Linux]

資料來源: https://www.youtube.com/watch?v=II7L8rpJ_6g
https://github.com/nodesource/distributions/blob/master/README.md
https://nodejs.org/en/about/

GITHUB:https://github.com/jash-git/How-To-Install-Node-JS-In-Ubuntu-Linux

$sudo apt-get install curl
$sudo apt-get install python-software-properties
#curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
$curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
$sudo apt-get update
$sudo apt-get install -y nodejs
$nodejs -w
$npm -w
$gedit app.js
	const http = require('http');

	const hostname = '127.0.0.1';
	const port = 3000;

	const server = http.createServer((req, res) => {
	  res.statusCode = 200;
	  res.setHeader('Content-Type', 'text/plain');
	  res.end('Hello World\n');
	});

	server.listen(port, hostname, () => {
	  console.log(`Server running at http://${hostname}:${port}/`);
	});
$nodejs app.js	