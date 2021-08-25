# Ano.js
A discord.js clone but more simple and have more features.
<div align="center">
</div>

## Example usage:
```js
const Ano = require('ano.js');
```
## Example Format:
```js
const Bot = new Ano.Bot({
  token: TOKEN, 
  prefix: PREFIX
  owners: ['Owner_ID','Owner_ID_2']
})
```

## Note: The format is not official we may change it eventually.


## Commmand Format (not official)

```js

client.command({
  name: "hi",
  aliases: ['hello'], // if none put nothing
  run {
  messag.send('Hi ${message.author.username}')
  }
})
```

Note: basically none of this is official till otherwise
