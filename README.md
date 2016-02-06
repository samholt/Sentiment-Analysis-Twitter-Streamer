#Twitter Streamer 

Streaming Tweets using Nodejs,Express,socket.io in backend,MongoDb as Database,AngularJs in frontend without using third-party module for authorization.


##Features 

 - Browser : Fetch Any Url Content 
 - Github : Fetch Github Repositories of any User
 - Twitter : Get Streaming Tweets on Searched Keyword
 - Implemented OAuth Encryption: auth.js 

 	+ https://dev.twitter.com/oauth/overview/authorizing-requests
	+ https://dev.twitter.com/oauth/overview/creating-signatures

 		* parameters are sorted and percent encoded => get parameter string
 		* get signature base string using url,method & parameter string
 		*  get signature HMAC-SHA1 encoded using signature base string.


##Configuration 

- Download and Install Node : http://nodejs.org
- Download and Install mongodb : http://mongodb.org
- Make directories for Mongodb data C:\data\db 

- Clone this repository using Git Bash: 

```ruby
	git clone https://github.com/aqfaridi/Twitter-Streamer.git
```

- Navigate to cloned directory, Update config.json with your developers twitter tokens.

	+ Go to http://dev.twitter.com 
	+ navigate to manage your app in footer http://apps.twitter.com
	+ Create new app, Fill up information asked
	+ Go to keys & access tokens tab, generate access token
	+ Twitter application key:consumer key & secret are application specific to make api calls

- open cmd prompt: Install all dependencies :

```ruby
	npm install express 
	npm install body-parser 
	npm install crypto
	npm install ejs
	npm install mongodb
	npm install socket.io  
```

- Run Mongo Server
```ruby
	mongod
```

- Run Node Server
```ruby
	node app
```
- Goto Browser : 

```ruby
	http://localhost:8000
```
