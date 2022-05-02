# Welcome to the IRC Docs!

Welcome to the Liberorum IRC Documentation. This documentation aims to give some insights, and also provide some useful commands.

## How do I connect?

You can connect to our IRC server on `irc.hahota.net`/`6697`(TCP). Only TLS connections are allowed, meaning `6667` won't work.

## Nicknames, registration:

Please notice that it is very, very important to choose your nickaname **before** connecting. On our server, your nickaname equals your username, and real name. Upon registering, you'll register this nickname for yourself. From that point, it can't be registered by anyone else, and you'll be the only one to hold that nickname.

Without registering, you won't be able to connect to any channels. This is protection against spam, and also prevents user spoofing.

To register an account for yourself;

1. Choose your preferred name, and hit connect.
2. DM nickserv: `msg nickserv register hunter12` (make sure to replace hunter12 with your preferred password).

## Login:

After registering, you'll might disconnect at some time. 

On our server, it is very important that you authenticate your account during the initial IRC handshake, otherwise you won't be able to use your previusly registered username. Our preferred mehanism for this is `SASL`, but you can also use the `PASS` command. Set the server password field to `username:hunter12`.

## Message sending:

On our server, by default, upon connecting a channel, the server sends the previus `100` messages to your client. This can be disabled, with the following command: `msg nickserv set autoreplay-lines 0`.

## Futhermore:

Please see our other wiki pages.