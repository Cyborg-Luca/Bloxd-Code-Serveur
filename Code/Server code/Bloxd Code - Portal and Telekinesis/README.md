# Bloxd Code - Staff Tools and Teleports (Part 4)

This repository contains the official script for the tutorial "Code pour Serveur - Partie 4". 
This code is designed for Bloxd.io private servers using the scripting API.

## Configuration

You can customize the script by editing the constants at the top of the file:

### Staff & Items System
- Staff Pass: Only the staff can walk through portals and code blocks.
- Fireball (Grab): Click a player to catch them. They will follow your gaze.
- Iceball (Launch): While holding a player, click to launch them away (Force 88).

### Teleportation System (Positions)
To change where players are teleported, modify the TELEPORTS constant:
- Trigger: The middle values [12, 13] are the X or Z coordinates that trigger the teleport.
- Destination: The last values [9, 1, -25] are the X, Y, and Z coordinates of the arrival.

## Staff Configuration

const STAFF = {
    OWNER: "Cyborg_Luca",
    CO_OWNERS: {
        "BOYhumanSigma": "yellow",
        "X_belle_fleur_677_X": "pink",
        "BestWizard119": "cyan"
    },
    ADMINS: {
        "Lord_Petit_Gueff_X": "Black"
    }
};

## Teleport Setup (Change Positions here)

const TELEPORTS = {
    Obsidian: [
        // Format: [ID, [Trigger_Pos], [Dest_X, Dest_Y, Dest_Z]]
        [1, [12, 13], [9, 1, -25]],
        [5, [-8, -9], [-53, 400, 50]],
        [52, [-53, -52], [-4, 400, 8]],
        [5, [0, 1], [-117, 400, 50]],
        [21, [-1787, -1786], [-5, 400, 52]]
    ]
};

*Developed for server management by Cyborg_Luca.*