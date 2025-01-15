# Grim Harvest spell effect automations

Automated the usage and effects for the Grim Harvest spell with the alias `!gHarvest` available on my workshop: https://avrae.io/dashboard/workshop/668c158264b0e862999dd0f7

- THP auto rolled and added to caster once effect is utilized
- Automation CON Save buttons added to the target of Clumsiness or Weakness
- Fatiguing exhaustion will increment and target dies if it reaches 6 levels
- Vampiric THP (half damage to 1 target) will be compared to GH THP and current THP
- Whithering damage factors in necrotic resistance/immunities

**Grim Harvest Documentation**

Usage: `!gHarvest [options] [effect] -t <target>`
- No arguments: shows this help.
- Must be in combat.

**Effects:** clumsiness, fatiguing, vampiric, weakness, withering

**Options:**
- `-l <level>` (min 6): Set spell level
- `arcanum`: Use Mystic Arcanum slot
- `-i`: Ignore slot/arcanum cost
- `-t <target>`: Set target

*withering:*
- `-die <die type>` (default d6) 
- `-rr <#>` number of hits from a single cast (e.g. hits with eldritch blast).
*vampiric:* 
- `-dmg <amount>` damage applied to one target | half will be used for THP.

Steps:
1. **One-Step**: `!gHarvest <effect> -t <target> [options]` can cast + apply in one go.
2. **Two-Step**: 
- `!gHarvest -t <dying target> [options]` to cast **Grim Harvest** and gain the effect on caster for 10 rounds.
- Then `!gHarvest -t <target> <effect> [options]` to apply that effect & gain THP.
