@title = "Riseup Chat"
@nav_title = "Chat"

## What is XMPP?

XMPP is an open standard for instant messages as well as voice and video chat. With XMPP, you can send and receive messages between users on thousands of different chat providers.

## Using Riseup's XMPP service

Your riseup.net email address also serves as your XMPP address. For someone to send you an XMPP message or buddy request, they just need to send it to `username@riseup.net`.

In order to configure a [[XMPP client => chat/clients]], you need this information:

- **protocol**: "xmpp"
- **account**: `username@riseup.net`
- **password**: your [[riseup-password]]

It is very important that you configure your client to **always require encryption**. Some clients have a setting "encryption if available". Even though the riseup.net servers require encryption, if your client is configured to use "encryption if available" an attacker can easily acquire your password.

Some XMPP clients will ask for your username and domain separately. In this case, you would specify:

- **username**: `username`
- **domain**: `riseup.net`

For tutorials on specific clients, see our [[XMPP client => chat/clients]] page.

## Connecting to multi-user chatrooms

When connecting to or creating chatrooms on Riseup's XMPP network, the syntax should be:

- `your-room-name@conference.riseup.net`

If you need to specify the room separately, do this:

- chatroom: `your-room-name`
- domain: `conference.riseup.net`

Do NOT use  `your-room-name@riseup.net`

### using rooms in Pidgin

If your are connected via [[pidgin]], to join or create a chatroom, click `Add room` in the `Buddy` menu.

- Room: `your-room-name`
- Server: `conference.riseup.net`
- Handle: `your-nick`
- Password: [optional]
- Alias: [optional]
- Group: [optional]

Click `Ok` and have a look at the buddy list. You should see a group `Chat` with your room.
Right click on it and select `join`.

For testing, you can select `riseup.net` as room name and join it.

## For added security

1. For added security, access our XMPP server via the [[Riseup VPN => vpn]].
1. Use our [Tor hidden service](https://www.torproject.org/docs/hidden-services.html.en) look for `xmpp.*.onion` at [[Riseup's onion services pages->tor#riseups-tor-hidden-services]].
