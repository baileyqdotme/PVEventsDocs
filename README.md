# Project Volt Event System

- **`/event` (Main Command)**
 - `/event alive` - Displays the number of alive players + their IGNS in a list
 - `/event broadcast` - Displays a message across the Project Volt network ( OBSOLETE - DON'T USE )
 - `/event end` - Ends the current event without a winner
 - `/event host` - Toggles your host status
 - `/event reload` - Reloads event data from config & db ( Don't use )
 - `/event resettoggle` - Resets all the toggles in the event (e.g. block break, pvp, player damage)
 - `/event revivaldata` - Used by console to edit db entries for a player's revivals ( Don't use, ask admin to do it )
 - **`/event set` **
  - `/event set host` - Sets the host's username ( Not used anymore - for display )
  - `/event set hosting` - Sets the method for hosting this event (e.g. minecraft chat, twitch, dc stage)
  - `/event set jail` - Sets the position for the event jail ( Don't use, ask admin to do it )
  - `/event set link` - Sets the link displayed on the actionbar when youtube or twitch are selected
  - `/event set name` - Sets the name of the event visible on holograms, tab & chat messages
  - `/event set prize` - Sets the prize for the event visible on holograms, tab & chat messages
  - `/event set spawn` - Sets the spawn for all players to be teleported to at the begining of the event ( Don't use, ask admin to do it )
  - `/event set start` - Sets the start for the event, used like: `/event set start 1d 2h 3m 4s`
 - `/event start` - Starts the event
 - **`/event toggle`**
  - `/event toggle BLOCK_BREAK (true/false)` - Toggles players being able to break blocks
  - `/event toggle BLOCK_PLACE (true/false)` - Toggles players being able to place blocks
  - `/event toggle FALLING_BLOCK_DEATH (true/false)` - Toggles players being instantly killed when hit by a falling block (used commonly during anvil drop)
  - `/event toggle LAVA_DEATH (true/false)` - Toggles players instantly dying in lava
  - `/event toggle PLAYER_DAMAGE (true/false)` - Toggles the players ability to take damage
  - `/event toggle PVP (true/false)` - Toggles pvp
 - `/event togglerevives (true/false)` - Toggles people's use of revivals they've either won from events or paid for
 - `/event tpall` - Teleports all alive players to you
 - `/event tpalldead` - Teleports all dead players to you
 - `/event visibility (ALL/HOST/NONE)` - Toggles the event visibility for all players

- **`/revive`** ( Main Command )
 - `/revive all` - Revives all players ( Including hosts - not recommended )
 - `/revive dead` - Revives all dead players ( Including hosts - not recommended )
 - `/revive gui` - Brings up the revival gui that players see when they run the command or use the revivals NPC
 - `/revive last` - Revives all players that died in the last 45 seconds
 - `/revive player (Username)` - Revives the player by that username
 - `/revive random` - Revives a random player ( Bit buggy as it includes alive players & hosts )

**- `/arena`** ( Main Command )
 - `/arena configure` - Configures the arena based on your WE selection ( DON'T USE - ASK AN ADMIN TO DO IT )
 - `/arena reset` - Resets the arena floor to Pink Concrete & Pink Concrete Powder
 - `/arena select`
  - `/arena select ARENA` - Sets the current arena as your WE selection
  - `/arena select ARENA_FLOOR` - Sets the current arena floor as your WE selection
  - `/arena select ARENA_WALLS` - Doesn't work - DONT USE
  - `/arena select ORIGINAL` - Selects the original arena as your WE selection ( arena without being shrunk thru `/arena shrink` )
 - `/arena  shrink (BLOCK AMOUNT)` - Shrinks the arena by the amount specified - **It can get laggy so tell players to get to the middle or teleport them to the middle as there is particles arround the side on all blocks that are no longer part of the arena**

**- `/blockshuffle`** ( Main Command )
 - `/blockshuffle config` - Configures block shuffle ( Run after you started the event)
 - `/blockshuffle round` - Starts a "round" ( Basically tells the player the colour that was randomly selected and starts the countdown )
 - `/blockshuffle timings`
  - `/blockshuffle timings blockCountdown (TICKS)` - Sets the amount of time **IN TICKS** (20 ticks = 1 second) players have to react until blocks are removed 
  - `/blockshuffle timings blockStayTime (TICKS)` - Set the amount of time **IN TICKS** the blocks stay removed/air
  - `/blockshuffle timings reset` - Resets the timings to default 
