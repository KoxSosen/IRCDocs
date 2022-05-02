# General

## Default channel modes:

Default channel modes are: `+RnC`.

## Creating your own public channels.

Feel free to create your own channels, and use them for your needs. Upon creating a channel, you'll become the owner of that specific channel, meaning you'll have the rights to control the permissions, the topic, the channel history, and many more in that channel.

For commands, please refer to our [commands](https://ircdocs.hahota.net/commands) page.

## Creating a private/invite only channel.

You may wish to create your own private channel. Private channels are only viewable by people you invite, and you. (and network operators).

To make a channel private, use the `+i` mode. If you have any bots, they'll have to be added as well.

First, register a channel, and then set it as invite only. Then use the invite command as shown above:

* - `/msg ChanServ register #privatechannelname` - Register your channel.
* - `/mode #privatechannelname +i` - Set it as invite only.
* - `/mode #privatechannelname +i username` - Invite `username` to the channel.

At this point, `username` will be able to join the channel just like any other: `/join #privatechanelname`.