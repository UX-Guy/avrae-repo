**Description**
You reap the life force of a dying creature and use it to empower the next spell you cast. Your target must be at 0 hit points and dying or must have died within the last round. If the target is dying, it must succeed on a Constitution saving throw or die.

The next time you cast a spell, you gain 1d10 + your spellcasting ability modifier in temporary hit points and can choose one of the following effects to inflict on the target in addition to the usual effects of the spell you are casting. If you do not cast another spell within 1 minute of casting this one, the effect is lost.

**Actions Available:**

Clumsiness, Fatiguing, Vampiric, Weakness, Withering

**Clumsiness**
Your target's speed is halved for 1 minute, and it has disadvantage on Dexterity ability checks and saving throws. At the end of each of its turns, it can make a Constitution saving throw. If it succeeds, the effect ends.

*Usage:*

`      -t target` Set target for the effect

**Fatiguing**
Your target must make a Constitution saving throw, gaining 1d4 levels of exhaustion on a failed save or 1 level of exhaustion on a successful one.

*Usage:*

`      -t target` Set target for the effect

**Vampiric**
You recover a number of hit points equal to half the damage you dealt. If you dealt damage to multiple creatures, you recover half the amount of damage you dealt to one of the targets.

*Usage:*

`      -t target` Set target for the effect
`    -amt damage` Damage applied to one target | half will be used for THP

**Weakness**
The target deals the minimum possible damage on melee attacks, if it hits, for 1 minute. At the end of each of its turns, it can make a Constitution saving throw. If it succeeds, the effect ends.

*Usage:*

`      -t target` Set target for the effect

**Withering**
You deal an extra 4 dice of damage of the same type as the damage dice of the spell and all damage dealt by your spell becomes necrotic damage.

*Usage:*

` -choice dieSize` (default d6) Damage die used by the spell 
`      -t target` Set target for the effect
`    -amt hits  ` (default 1) Number of times the spell damaged the target
