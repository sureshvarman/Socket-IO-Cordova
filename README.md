Socket-IO-Cordova
=================

Simple Socket IO+cordova program for web and mobile

Nodejs
-------------------------------------------------------------------------------------------------------------------------
	Nodejs is a server side javascript platform on Chrome's JavaScript runtime. 

	Advantages	
	----------
	Event-Driven
	Non-blocking I/O
	Light Weight Because of Javascript
	
For further Details and installation Guide visit : http://nodejs.org/

	
Cordova
--------------------------------------------------------------------------------------------------------------------------
	Apache Cordova is a platform for building mobile applications without the knowledge of native code.
	
	Advantages	
	----------
	Multi-platform Mobile application Development with HTML5, Javascript, CSS.
	apache cordova engine takes care of native code.
	Easy for web developers to create a mobile application without native code knowledge
	
For Further Details visit : http://cordova.apache.org/
	
Installing Cordova in Nodejs and creating project visit : http://docs.phonegap.com/en/3.5.0/guide_cli_index.md.html#The%20Command-Line%20Interface

Simple Socket IO+cordova program for web and mobile
------------------------------------------------------------------------------------------------------------------------------
Install 'Socket.io' module and 'express' module using npm as

	C:\>npm install socket.io
	C:\>npm install express
	
Create New Project in cordova using command line

	C:\> cordova create chat com.chat.app Chat
	
The above command create a simple cordova project with folder structures as follows
					Chat
					 |
					 |--->hooks
					 |--->platforms
					 |--->plugins
					 |--->www
					 |--->config
					 |
	The WWW is the root folder where we are going to spend our development Time
	
	copy the directory www from repository and replace that with your www folder
	
	NOTE : For who are not familiar with nodejs you have to copy your node modules socket.io and express to WWW/js/node_modules
			and who have to start your nodeserver using following command
			C:\chat\www\js>node nodeserver.js
			
	nodeclient.js
	-------------
	Change your IP address as follow in nodeclient.js file
	var socket = io.connect( 'http://IPAddress:1034' );
	This IPAddress shouldn't be localhost give your Valid IP address if you are using mobile broadband 
	check your public ip using http://whatismyip.com/ and pass that IP
