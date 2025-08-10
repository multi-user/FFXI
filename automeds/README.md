**AutoMeds** is a Windower addon that automatically uses medicine when your character is affected by specific debuffs.

## Features

- Automatically uses the correct item for common debuffs.
- Automatically skips item use if the item isn’t in your inventory.
- Retries item use until the debuff is cleared.
- Automatically stops once the debuff is gone.
- Tracks debuffs on your character.
- IPC Multi-Character Support:
	1. Broadcast debuff info to alts (trackalt).
	2. Notify when Sneak/Invisible is wearing off (sitrack).
- Configurable buff tracking list.
- Aura Awareness:
	1. Distance-based aura check will continuously scan nearby targets and their debuff within in your aura list.
	2. Distance check only triggers if a matching target is within your set range (default: 20 yalms).
	3. Auto-suppress item usage if a debuff is within in your aura list is detected nearby.
	4. Targets must be added to the aura list for Aura Awareness to work.
	5. Better than Smart Aura Block if you know what debuff you'll be encountering.
- Smart Aura Block:
	1. Disabled by default.
	2. Works even if Aura Awareness is disabled.
	3. Pauses item use for a set duration if repeated attempts fail to remove a debuff (default: 2 attempts then a 120 second pause).
	4. Pause duration can be set between [60 - 600] seconds.
	5. Each debuff has it's own pause duration counter.
	6. Pause duration resets when the debuff debuff is no longer active.
	
## Commands

Do not type [ ] when using commands:

List commands: //ameds help

- //ameds watch [buff] - Track a debuff
- //ameds unwatch [buff] - Untrack a debuff
- //ameds list - Show tracked debuffs
- //ameds toggle - Toggle Automeds On/Off
- //ameds trackalt - Toggle alt broadcast
- //ameds sitrack - Toggle Sneak/Invisible wear tracker
- //ameds aura on|off - Enable/Disable Aura Awareness
- //ameds aurasmart on|off - Enable/Disable Smart Aura Block
- //ameds aurablock [seconds] - Set pause duration [60 - 600]
- //ameds auradistance [yalms] - Set distance detection for Aura Awareness
- //ameds auraadd "[target]" [debuff] - Add target for Aura Awareness
- //ameds aurarem "[target]" [debuff] - Remove target from Aura Awareness
- //ameds auralist [target] - List aura sources
