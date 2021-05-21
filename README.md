# dbd.js-discord-bot

A Multipurpose Discord Bot with dbd.js

### ⛓️ Installation and Setup
- Go to `index.js` and keep your status and token 
> How to do it?
```js
const bot = new dbd.Bot({
  mobile: false, //U can change to true if u wanna have a mobile status
  token: "XXXXXXXXXX", //CHANGE with your TOKEN
  prefix: ['$getServerVar[prefix]', '<@!$clientID>', '<@$clientID>'] 
})
```
- After that scroll down and change status
> Status Example
```js
bot.status({
    text: `with $serverCount servers`, // put any text
    type: "PLAYING", // LISTENING, PLAYING, WATCHING, COMPETING
    status: "online", // online, dnd, idle, invisible
    time: 75 // amount of times where you can change the bot status (if have multiple statuses)
    })
```
- For Multiple Status
> Multiple Status Example
```js
bot.status({
    text: `AMONG US`,
    type: "COMPETING",
    status: "online", 
    time: 75 
    })
    
bot.status({
    text: `music`, 
    type: "LISTENING", 
    status: "online", 
    time: 75
    })

bot.status({
    text: `with $serverCount servers`, 
    type: "PLAYING", 
    status: "online", 
    time: 75
    })
```
- For Streaming Status
> Streaming Status Example
```js
     bot.status({
     text: "text", 
     type: "STREAMING", 
     url: "enter url/link"
       })
```
- After that go to `vars.js`
```js
module.exports = ({
  prefix: "!", // Change with your prefix
    xp: "0",
    level: "0",
    req: "50",
    expcd: "45",
    leveling: "enabled", //U can disable if u want
    money: "0"
  })
```
- Fill with your steps
After that go to terminal and type `npm i dbd.js@2.2.6` and `npm i dbd.db` and after do `npm i dbdjs.db` and to start the bot type `node index.js`
    
