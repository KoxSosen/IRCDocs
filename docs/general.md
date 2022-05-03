# General

## Default user, channel modes:

The default user modes are: `+iRT`. See `/QUOTE HELP umodes` for explanation. 

Default channel modes are: `+ntCR`. See `/QUOTE HELP cmodes` for what each option means.

## IP cloaking:

On our server all IP's are cloacked. What this means, is that noone will be able to see your IP, or the hostname you're connecting from. Not even channel OP's. An example ip would be `84781476174x.irc.hahota.net`.

## Persistent message history:

On our server, we store everything you send and for later playback, both in private messages, and both in channels. 
In every channel, history can be requested with the `/history <timeframe>` command. For channel operators, you can opt-out this feature.

For private messages, this is enabled as well, but you have the option to disable this behavior.

To corporate with data privacy regulations, you may request your data to be deleted from this, or these databases, however we can't guarantee any data deletion from connected user's clients.

## Always on:

You can set your status to show up as "always on", even if you aren't connected to the server. When connecting back, the server will only try to send the messages to your client that you missed. Enable this with `/msg NickServ set always-on true`.

Our choice of server software, [Ergo](https://github.com/ergochat/ergo/) supports setting different Device ID's. Device ID's can be used to track messages, eg you can use a different device ID for you phone and PC, and the server will automatically track which messages you missed/viewed on each device, and sync them. By default this is **not** enabled. You have multiple options to set a device id. You can either add it to your SASL username (`exampleuser` -> `exampleuser@pc`), to your IRC ident, and you can add it to your `PASS` commnad as well (`exampleuser:hunter12` -> `exampleuser@pc:hunter12`).

If you have only one device, you can use the `/msg NickServ set autoreplay-missed true` command.

## Email verification:

Email verification is disabled within our system. It might be implemented in the future.

## Limits, throttling:

Multiple kinds of limits are implemented within our system to prevent spam, and many more. For more details, please ask the network operators.

## Multiclient

Multi client compatibility is enabled, and is allowed.

## Creating your own public channels:

Feel free to create your own channels, and use them for your needs. Upon creating a channel, you'll become the owner of that specific channel, meaning you'll have the rights to control the permissions, the topic, the channel history, and many more in that channel.

For commands, please refer to our [commands](https://ircdocs.hahota.net/commands) page.

## Creating a private/invite only channel:

You may wish to create your own private channel. Private channels are only viewable by people you invite, and you. (and network operators).

To make a channel private, use the `+i` mode. If you have any bots, they'll have to be added as well.

First, register a channel, and then set it as invite only. Then use the invite command as shown above:

* - `/msg ChanServ register #privatechannelname` - Register your channel.
* - `/mode #privatechannelname +i` - Set it as invite only.
* - `/mode #privatechannelname +i username` - Invite `username` to the channel.

At this point, `username` will be able to join the channel just like any other: `/join #privatechanelname`.