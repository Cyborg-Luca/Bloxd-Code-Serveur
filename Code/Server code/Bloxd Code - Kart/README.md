# Bloxd Code - Staff Kart System (Part 6)

This repository contains the official script for the tutorial "Code pour Serveur - Partie 6".
This code is designed for Bloxd.io private servers using the scripting API.

## Configuration

You can customize the script by editing the constants at the top of the file:

### Staff System 

- Access Control: Only players listed in the STAFF object can use the Kart commands.
- Security: The script checks the player's name before executing any visual or physical changes. 

### Kart Customization 

- Commands: Use :CKART to spawn the vehicle and :CUNKART to remove it.
- Speed Tuning: To change the speed, look for the "Speed" effect line. Change the value 10 to a higher or lower number to adjust the velocity.
- Visuals: The script attaches a 3D Kart mesh to the player and changes their posture to a driving pose.

## Staff Configuration

Modify this object to add your team members:

    const STAFF = {  
	OWNER: "Cyborg_Luca",
    CO_OWNERS: ["CO-OWNER1", "CO-OWNER2", "CO-OWNER3"],
    ADMINS: ["ADMIN"]
};


## Speed Configuration (How to change)

To modify the Kart's speed, locate this specific line in the code:

// Replace '10' with your preferred speed level
api.applyEffect(id, "Speed", null, { inbuiltLevel: 10 });

*Developed for server management by Cyborg_Luca.*