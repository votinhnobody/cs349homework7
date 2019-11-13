# CPSC349-HW7

_to run project_

#install parcel:

install  parcel: npm install -g parcel-bundler

npm run build

npm run watch
Open another command: npm run dev

http://localhost:3000/
go to dev Console to see message

parcel app/scripts/src/app.js -o app/scripts/dist
parcel app/scripts/src/main.js -d app/scripts/dist
wathify -v -d app/scripts/src/main.js -o app/scripts/dist/main.js

in package.json:
"build": "parcel build app/scripts/src/main.js -d app/scripts/dist",
"watch": "parcel watch app/scripts/src/main.js -d app/scripts/dist"





#install Node.js
- install Node.js
- create package.json file (in project directory): npm init
press enter to accept default
	+ in json file: in "scripts" section, add:
		"start": "node index.js"

- to start Node server: npm start
	+ in brower: localhost:3000
- to stop program: Control-C
- add third-party modules: npm install --save
ex: npm install --save ws (websockets)
- install mime: npm install mime

#install WebSocket
Setting Up WebSockets To set Chattrbox up with WebSockets, you are going to:
1. install the ws module: npm install --save ws
2. create a WebSockets server
3. add chat functionality to the server
4. accommodate new users by having the server send them the message history


--- testing WebSockets Server ---
using wecat, install globally: npm install -g wscat
run nodemon in terminal: npm run start or npm run dev

Open another terminal: wscat -c ws://localhost:3001
or wscat -c http://localhost:3001
Then, start chatting
