# Bloxd Code - Black screen (Part 7)

This repository contains the official script for the admin command system used on Cyborg_Luca's Bloxd.io private server.
This code is designed for Bloxd.io private servers using the scripting API.

## Configuration

You can customize the staff list by editing the `STAFF` object at the top of the script:

### Staff Setup
**OWNER:** Only one owner is supported. Set it to your username.
**CO-OWNERs:** Add or remove co-owners and their associated chat color.
**ADMINs:** Add or remove admins and their associated chat color.

## Available Commands

All commands are triggered by prefixing a message with `:`.
**:CBLACK `<player>`** — Applies a black screen to the target player.
**:CUNBLACK `<player>`** — Removes the black screen from the target player.

## Script Implementation

This snippet shows the core logic triggered when a player sends a chat message:

```js
/**
 * Event: Player Chat
 * Intercepts messages starting with ":" and routes them to the command handler.
 */
onPlayerChat = (id, msg) => {
    if (msg.startsWith(":")) {
        Y(id, msg);
        return false;
    }
    return true;
};

*Developed for server management by Cyborg_Luca.*
	