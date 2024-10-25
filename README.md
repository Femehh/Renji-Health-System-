Advanced Health System for Unity
The Advanced Health System script provides a comprehensive health, role, and damage management system for Unity. Customize player roles, health, and damage with easy-to-configure settings. This script is ideal for games requiring diverse roles, such as RPGs or multiplayer experiences.

Features
Customizable Player Roles: Define unique health, speed, damage, and appearance for each role.
Armor & Health Mechanics: Manage health, armor, and healing with ease.
Damage Items: Create items that deal damage with sound effects and customizable damage properties.
Respawn System: Players respawn after death with effects and sounds.
Health Bar Display: Shows a health bar above each player.
Configurable Healing Over Time: Regenerate health at set intervals.
Setup Instructions
Step 1: Adding the Script to Your Project
Download AdvancedHealthSystem.cs and place it in your project’s Scripts folder.
In Unity, select your Player GameObject (or the character GameObject you want to add health and role features to).
Attach the Script by dragging AdvancedHealthSystem.cs onto the Player GameObject.
Step 2: Configuring Basic Player Settings
Player Identity: In the Inspector, set playerName and playerLevel to identify each player. These can be used to adjust stats if desired.
Step 3: Creating and Customizing Player Roles
In the Role Settings section:
Add Roles by expanding PlayerRoleSettings.
For each role, define:
roleName: Name of the role (e.g., “Citizen”).
healthMultiplier: Multiplies the player’s base health.
damageMultiplier: Increases or decreases damage dealt by the player.
speedMultiplier: Changes player movement speed.
roleColor: Color that identifies the role in-game (applies to the player’s material).
Step 4: Setting Health & Armor
Health Settings:

Set the player’s baseHealth.
This value will be adjusted by each role’s healthMultiplier.
Armor Settings:

Enable Use Armor by checking useArmor.
Set armorReductionPercentage to control how much armor reduces incoming damage (e.g., 20% reduction).
Step 5: Customizing Damage Items
Under Item Damage:
Add damage items, such as weapons, with unique properties.
Each item has:
itemName: The item’s name (e.g., “Knife”).
damageAmount: How much damage it deals.
ignoresArmor: If checked, the item will bypass the player’s armor.
impactSound: An optional sound effect that plays when the item is used.
Step 6: Enabling Health Regeneration
Healing Over Time: Check enableRegen to allow health regeneration.
Set regenAmount (health gained per interval).
Set regenInterval (time interval in seconds for each regeneration tick).
Step 7: Configuring Death, Respawn, and Visual Effects
Death Settings:

Attach a deathEffect (e.g., a particle effect) that plays upon player death.
Attach deathSound to play a sound when the player dies.
Respawn Settings:

Check respawnOnDeath to allow players to respawn after death.
Set respawnTime (in seconds) before the player respawns.
Add a respawnEffect if desired.
Step 8: Adding Health Bar UI
UI Display Settings:
Check showHealthBar to show a health bar above the player.
Attach a Health Bar Prefab (e.g., a UI slider or bar) that will follow the player’s health status.
Usage
Example: Setting Up Roles
To add roles like Citizen and Mafia:

Go to Role Settings in the Inspector.
Add entries for:
Citizen: Set healthMultiplier to 1.0, damageMultiplier to 1.0, and choose a neutral color.
Mafia: Set damageMultiplier higher (e.g., 1.5) for stronger attacks and choose a distinct color.
Example: Taking Damage
To apply damage using a configured item:

Call ApplyItemDamage("Knife") to use the item’s damage settings.
The script will check for armor and apply effects based on ignoresArmor.
Code Structure
PlayerRoleSettings: Stores unique settings for each role.
DamageItem: Defines item-specific damage.
AdvancedHealthSystem: Main script for health, damage, and player role functionality.
Notes
Health Bar UI: Ensure you have a prefab ready to display health. It scales based on the player’s remaining health.
Role Colors: The player’s color updates automatically based on their role.
This setup provides a comprehensive role-based system for health and damage in Unity, perfect for complex multiplayer or role-playing games. Adjust settings in the Inspector as needed to fine-tune each role and gameplay experience.
