# Bloxd Code - Chat and Tableboards (Part 1)

This repository contains the official script for the tutorial "Code pour Serveur - Partie 1". This code is designed for Bloxd.io private servers using the scripting API.

## Configuration

You can customize the script by editing the constants at the top of the file:

### Chat System
- Automatic Ranks: Assigns prefixes for OWNER, CO-OWNER, and ADMIN roles.
- Custom Colors: Each rank has a specific color in the chat for clear identification.
- Message Formatting: Consistent visual style for all outgoing messages.

### Information Table
- Player Counter: Shows the real-time number of connected players.
- Staff List: Displays usernames of the owner and management team.
- Server Rules: Constant display of basic rules (no griefing, respect, specific zones).
- Auto-Refresh: The table updates every 5 seconds to ensure data accuracy.

## Staff Configuration

To modify staff members, edit the `STAFF` constant at the beginning of the code :

const STAFF = {
    OWNER: "YourUsername",
    CO_OWNERS: {
        "CO-OWNER1": "red",	
        "CO-OWNER2": "pink"
    },
    ADMINS: {
        "Admin1": "Black"
    }
};

*Developed for server management by Cyborg_Luca.*
