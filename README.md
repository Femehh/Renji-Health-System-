Advanced Health System
Overview
The AdvancedHealthSystem script allows you to customize player roles and assign them different health, speed, damage, and visual settings in Unity. Each role can have unique multipliers and color settings, making it easy to create diverse character types, from citizens to combat-ready characters like the mafia.

Key features include:

Customizable player roles with health, speed, and damage multipliers
Configurable health, armor, and healing mechanics
Support for item-based damage
Health regeneration over time
Respawn on death with effects and sounds
Health bar display
How to Use
Add the Script to Your Player GameObject

Attach the AdvancedHealthSystem script to the player character GameObject. This setup allows the player to have health, armor, and respawn mechanics.
Configure Player Roles in Inspector

In the PlayerRoleSettings section, you can add various roles like "Citizen," "Mafia," or "Doctor."
Each role has attributes such as:
roleName: The name of the role, e.g., "Citizen"
healthMultiplier: Adjusts health for each role
damageMultiplier: Adjusts how much damage they deal or take
speedMultiplier: Modifies speed
roleColor: Changes player color based on role
Adjust Base Settings in Inspector

Player Identity: Set player name and level, which can influence stats.
Health Settings: Define base health and initial values.
Armor Settings: Enable or disable armor, set the armor percentage reduction.
Damage Settings: Adjust cooldown between damage instances.
Healing Over Time: Enable health regeneration and set regeneration amount and frequency.
Define Damage Items

In the Damage Item section, create items that inflict damage, e.g., a “Knife” with a specified damage amount and sound effects.
Respawn and Death Visuals

Add death and respawn effects, sounds, and adjust respawn times to enhance gameplay experience when players die and respawn.
Health Bar Display

Enable UI Display Settings to show a health bar above the player, which scales based on health percentage.
Features Explained
Dynamic Roles: Each role can alter player health, speed, and attack power through customizable settings.
Health and Armor: Protects the player based on armor settings and allows fine-tuning of how armor reduces incoming damage.
Damage Cooldown: Prevents rapid damage in short intervals, providing balance.
Healing and Regeneration: Configurable health regeneration adds realism by restoring health gradually over time.
Damage Items: Integrate various weapons and items with different effects and sounds.
Respawn Mechanics: Automatic respawn after death with effects and sounds to keep players in action.
Health Bar UI: Displays real-time health changes to players.
Example of Configuring Roles
Add AdvancedHealthSystem to your player GameObject in Unity.
Expand Player Roles in the Inspector and create roles:
Citizen: Set healthMultiplier to 1.0, speedMultiplier to 1.0, damageMultiplier to 1.0, and roleColor to white.
Mafia: Set higher damageMultiplier for stronger attacks, and a different roleColor.
Doctor: Slightly lower damageMultiplier, unique roleColor, and enable a healing item.
Additional Notes
Role Color: Automatically applies when a role is assigned.
On Damage: Plays specific sounds and updates health visually.
Regen: Automatically starts when enableRegen is true.
This script makes it easy to integrate a fully-featured health and role system into any Unity game, making it ideal for RPGs, combat games, and any multiplayer game where role diversity is key. Adjust settings in the Inspector for immediate gameplay effects, and feel free to extend the script for even more custom roles and effects!
