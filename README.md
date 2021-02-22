# 24/7 discord bot template

# option 1 for self hosting:

in the .env file change your-token to your discord bots token. Or you could use the config.json and put your token in it (i use the config.json)

go to repl.it and import this repo and run the repl. there should be some packager files now.

then copy the url at the pot of the output and copy it. go to uptimerobot.com and make an account or sign in. make a monitor and choose https, make a name, and put the url in the url slot. then press the create monitor button and your bot will be online 99.9 percent of the time!

you can put your bot files in the repl like commands and stuff, but make sure there is not any files named index.js or .env (.env is okay just move the contents of it over to the .env that comes with your bot.)

# option 2 for self hosting: (DEFINITLY THE EASIER OPTION)

put the following code in your index.js file on repl or what ever you host with:

var _247DiscordJsBotTemplate = require("@chelms21/24-7-discord.js-bot-template")

# including bot code

now you can put in your bot code for your discord bot

# 24-7

run your repl (assuming you are using repl it) or whatever your code is in

get the url and put it in uptime robot like in the above option. (this is why i recommend repl.it because it gives you a normal url instead of a localhost one)

# put it all together

create a config.json file and put the following code (or .env code is below the config.json code)

{
  "token": "your_token_here"
}

# .env code:

# index.js:  

remove:  const { token } = require('./config.json')     and      client.login(token)
add: client.login(PROCESS.env.DISCORD_TOKEN)

# .env:

add:  DISCORD_TOKEN=your_token_here
