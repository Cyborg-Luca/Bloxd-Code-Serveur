# Bloxd Code - Respawn Code (Part 5)

This repository contains the official script for the tutorial "Code pour Serveur - Partie 5". 
This code is designed for Bloxd.io private servers using the scripting API.

## Configuration
You can personalize the player's connection experience by modifying the parameters within the script:

### 1. Interface Customization
Respawn Button Text: Change the label that appears on the death screen.

Branding: Set your server name or a custom message to greet players.

### 2. Gameplay Timing
Respawn Delay: Adjust the time (in seconds) a player must wait before they can rejoin the action.

### Script Implementation

##This code snippet manages the logic triggered when a player joins the server:
/**
 * Event: Player Join
 * Handles UI customization and respawn settings.
 */
onPlayerJoin = (myId) => {
    // Set custom text for the respawn button
    api.setClientOption(myId, "respawnButtonText", "Serveur de Cyborg Luca");
    
    // Set the delay before respawning is possible (in seconds)
    api.setClientOption(myId, "secsToRespawn", 3);
};