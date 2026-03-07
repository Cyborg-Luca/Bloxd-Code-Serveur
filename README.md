# Bloxd Code - Chat and Tableboards (Part 1)

This repository contains the official script for the tutorial "Bloxd Code - Chat and notice board". This code is designed for Bloxd.io private servers using the scripting API.

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

By @Cyborg_Luca
