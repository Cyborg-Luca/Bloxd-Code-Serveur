# Bloxd Code - Guard System (Part 2)

This repository contains the official script for the tutorial "Code pour Serveur - Partie 1". This code is designed for Bloxd.io private servers using the scripting API.

## Configuration

You can customize the script by editing the constants at the top of the file:

### 1. Staff Members
Update the `STAFF` object with your team's usernames:
- `OWNER`: The main owner.
- `CO_OWNERS`: List of co-owners and their display colors.
- `ADMINS`: List of administrators.

### 2. Forbidden Items
Modify the `OBJETS_INTERDITS` array to add or remove restricted weapons or blocks.

### 3. Zone Coordinates
Zones are defined using `min` and `max` vectors `[x, y, z]`:
- `ZONES_BLOCS`: Areas where building is restricted.
- `ZONES_SAFE`: Areas where combat is disabled.

*Developed for server management by Cyborg_Luca.*