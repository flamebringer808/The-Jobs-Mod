# The-Jobs-Mod
Short Description:
Jobs Mod lets admins create custom jobs and assign them to players. Each job grants passive effects and item enchantments. Includes job creation, deletion, player assignment, and persistent data storage. Perfect for RPG servers.

---------

Description:
The Jobs Mod

Transform your server with customizable jobs that grant passive effects, auto-enchant items, add debuffs, define defeat-based quests with rewards, and expose player-usable commands with cooldowns and costs. Ideal for RPG and economy servers.

Features

Bold the keyword: Create Jobs: administrators define roles with custom effects, enchants, debuffs.
Quest System: add defeat quests per job and attach item/effect rewards.
Player Commands: per-job commands players can run; supports cooldowns and costs.
Debuffs: effect-based debuffs and permanent heart reductions.
Persistent Data: saves in world data, survives restarts.
Permission Control: admin-only setup commands (OP level 2 or Creative).

Admin Commands

Create/Delete/Assign/Strip:
/job create <name>
/job delete <name>
/job assign <player> <job>
/job strip <player>
Configure Passive Effects:
/job config <job> effect <effect> <level>
Configure Enchantments:
/job config <job> enchant <item> <enchant> <level>
Configure Debuffs:
/job config <job> debuff effect <effect> <level>
/job config <job> debuff hearts <count>
Configure Quests (defeat only):
/job config <job> quest passive defeat <entity> <count>
Configure Rewards:
/job config <job> reward passive item <item> <count>
/job config <job> reward passive effect <effect> <duration> <amplitude>
Create Player Commands:
/job config <job> commands create <cmdname> effect <effect> <duration> <amplitude>
/job config <job> commands create <cmdname> give <item> <count>
/job config <job> commands cooldown <cmdname> <ticks>
/job config <job> commands cost life
/job config <job> commands cost hearts temporary <count>
/job config <job> commands cost hearts permanent <count>
/job config <job> commands cost items <item> <count>

Perfect for creating role-based gameplay, server economies, and immersive multiplayer experiences.
