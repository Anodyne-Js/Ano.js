# Ano.js
A discord.js clone but more simple and have more features.
<div align="center">
</div>

## Example usage:
```js
const Client = require('ano.js');
const client =new Client(botToken, ['YOUR ID','OTHER ID'], '-');
//const client = new Client(botToken, ['YOUR ID','OTHER ID'], '-');
client.start();
client.on('ready', () => {
  /* eslint-disable no-console */
  console.log(`${client.user.tag} is ready
OWNER: ${client.owner}`);
});

client.command({
    name: "ping",
    aliases: ['pings', 'pong']
  },
  message => {
    message.channel.send('PONG!');
  });

client.command({
  name: "help",
  aliases: ["help", "commands"]
}, message => {
  message.channel.send(client.user.username + " Help list:\n")
})
