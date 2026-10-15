# Documentació del Bot de Discord
![Logotip de Discord](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Flogosmarcas.net%2Fwp-content%2Fuploads%2F2020%2F12%2FDiscord-Logo.png&f=1&nofb=1&ipt=c0f7cd6e97f4b7f7c0400995f51c2d1f95d1349f79233ecd3ce43fb0020eb313&ipo=images)
Pots registrar la teva aplicació al [Portal de Desenvolupadors](https://discord.com/developers/applications) de Discord
Per fer que el bot respongui, escoltem l'esdeveniment `messageCreate` i utilitzem el mètode `message.reply()`

```JavaScript
client.on('messageCreate', message => {
 if (message.content === 'ping') {
 message.reply('pong!');
 }
});
```