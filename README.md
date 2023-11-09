## MomentumAI

All new commands must be registered. To register a new slash command,
run the `deploy-commands.js` file before launching the bot.

```cmd
$ node deploy-commands.js
$ node index.js
```

We may set this up to run as a CRON job on the server at a regular interval (TBD)


`interactionCreate.js` logs the activity of the bot and the user interaction. This should point to a "backstage" channel, where moderators can monitor the activity of the bot right in the Discord server.