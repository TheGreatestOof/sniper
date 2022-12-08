<img width="64" height="64" align="left" style="float: left; margin: 10px 10px 0 0;" alt="Icon" src="https://imgur.com/dRSYp1f.png">

# Sniper

> An easy to run simple bot that lets you snipe messages in your Discord server.

## Setup

[Node.js 16.9.0](https://nodejs.org) or newer is required.

1. Run:

```bash
$ git clone https://github.com/TheGreatestOof/sniper.git
$ cd ./sniper
```

2. Create config.json:

```json
{
	"token": "<Your bot's token>",
	"application_id": "<Your application's id>"
}
```

3. Run:

```bash
$ npm i
$ npm run register [guild id]
$ npm run bot
```

> Note:
> Without specifying [guild id], the snipe commands will be available to all of your app's guilds. They will fan out slowly across all guilds and will be guaranteed to be updated in an hour (due to Discord's cache).
> 
> With [guild id] they will be available only within the guild specified and will update instantly.

## Top.gg Support

If you decide to host your wonderful snipe bot on top.gg, it can now post statistics like server count to the bot page.
But before you do this, the topgg-autoposter library must be installed.

```
$ npm i topgg-autoposter
```

In the field for 'your top.gg token', you need to enter the token from your bot dashboard's edit page -> webhooks. This is NOT the same as your Discord bot token.
You must add this in the index.js file present in the src folder. It's at the bottom of the file. 

## Dockerfile instructions
An [example Dockerfile](Dockerfile.example) has been included. Modify line 12 to change the guild id. If you want to make the bot global, simply comment out line 12.

# Privacy Policy

The use of this application ("Bot") in a server requires the collection of some specific user data ("Data"). The Data collected includes, but is not limited to Discord user ID values. Use of the Bot is considered an agreement to the terms of this Policy. 

## Access to Data

Access to Data is only permitted to Bot developer, and only in the scope required for the development, testing, and implementation of features for Bot. Data is not sold, provided to, or shared with any third party, except where required by law or a Terms of Service agreement. You can view the data upon request from TG#9456

## Storage of Data

Data is stored in a MongoDB database. The database is secured to prevent external access, however no guarantee is provided and the Bot owners assume no liability for the unintentional or malicious breach of Data. In the event of an unauthorised Data access, users will be notified through the Discord client application.

## User Rights

At any time, you have the right to request to view the Data pertaining to your Discord account. You may submit a request through the [Discord Server](https://discord.gg/ycMXtrpyrT). You have the right to request the removal of relevant Data.

## Underage Users

The use of the Bot is not permitted for minors under the age of 13, or under the age of legal consent for their country. This is in compliance with the [Discord Terms of Service](https://discord.com/terms). No information will be knowingly stored from an underage user. If it is found out that a user is underage we will take all necessary action to delete the stored data.

## Questions

If you have any questions or are concerned about what data might be being stored from your account contact `TG#9456`. For more information check the [Discord Terms Of Service](https://discord.com/terms).

## License

[MIT](https://tldrlegal.com/license/mit-license)


