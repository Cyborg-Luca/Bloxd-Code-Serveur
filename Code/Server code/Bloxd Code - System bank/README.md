# Bloxd Code - Economy and Shop System (Part 2)

This code is designed for Bloxd.io private servers to manage a banking system and a custom shop.

## Configuration

You can customize the script by modifying the constants and functions at the top of the code:

### Economy System (Bank and Shop)

- **Emerald Bank**: Uses "Emerald Blocks" as physical currency in the Moonstone Chest.

- **Shopping System**: Automatically converts harvested items (Bread, Apples, etc.) into Gold.

- **Money Transfer**: Includes a `:CLP` command to securely send Gold between players.

- **Balance Check**: Use the `:CLS` command to refresh the display.

### Visuals and Shop

- **Dynamic Scoreboard**: A side panel displaying the real-time Gold balance and server information. - **Custom Shop**: Pre-configured logic for purchasing "Double Barrel" weapons or enchanted equipment (Health level 5).

## Staff and Price Configuration

To modify the scoreboard or item prices, change the constants at the beginning of the code:

```javascript
const STAFF = {

OWNER: "Cyborg_Luca",

CO_OWNERS: { "BOYhumanSigma": "yellow" }
};

const items = {

"Bread": 10000000, 
"Apple": 4, 
"Wheat": 1
};

All the available enchantments that I found :

Health, Health Regen, Protection, Attack Speed, Critical Damage, Damage, Break Speed, Momentum,
Mining Aura, Mining Yield, Digging Aura, Farming Aura,  Farming Yield, Lumber Aura, Lumber Yield,
Arrow Speed, Arrow Damage, Quick Charge, Horizontal Knockback, Vertical Knockback, Knockback Resist, Stomp Damage

Developed for server management by Cyborg Luca.