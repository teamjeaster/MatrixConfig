# MatrixConfig

> The optimized config for [Matrix Anticheat](https://matrix.rip/).

![Built with oxygen](https://badgen.net/badge/built%20with/oxygen/green) ![for matrix free](https://badgen.net/badge/for%20free%20matrix/4.8.8/green) ![and premium](https://badgen.net/badge/and%20premium%20matrix/4.8.8/green) ![open issues](https://img.shields.io/github/issues/PhoenixDiscord/MatrixConfig.svg) ![last commit](https://img.shields.io/github/last-commit/PhoenixDiscord/MatrixConfig.svg)

**Warning: You should use `checks-free.yml` if you use the free version. Also, using the premium config won't get you premium features and will most likely crash Matrix.** If you have premium, see `checks-premium.yml`.

Joining the Discord server(s) is recommended because sometimes I'm too busy to update the config in 3 places.

### Terms
You can use this for anything, and modify it if you want to, but just please don't say that it's entirely yours and no one else contributed to it.

### Important thing to remember
Don't assume that this config will be perfect for your server out of the box - each server is different, you should tweak the config for your own needs.

Also, remember that in most cases with Matrix, it's either get a big amount of false kicks or make the detection a little bit more lenient.

I can't make your anticheat kick people seconds after they turn on their hacks without causing false positives if I can't even access the code. This ain't NoCheatPlus. We are still trying to make checks that cause a very small amount of false positives more strict.

### Recommended changes
1. `nofall.damage: true` -> `nofall.damage: false` (for minigame servers with fall damage disabled)

2. `hitbox.max-reach: 3.2` -> `hitbox.max_reach: 3.3` (if you have hitbox false positives **[makes hitbox detection more lenient!]**)

3. `killaura.modules.autoclicker.max_cps: 18` -> `killaura.modules.autoclicker.max_cps: (number from 8 to 24)` (decrease if your players don't click fast, or increase if they do. **don't go above 24!**)

4. `inventory.cancel_vl: 8` -> `inventory.cancel_vl: (number from 8 to 14)` (increase if the check causes false positives)

5. `fastuse.commands.32: ...` -> `fastuse.commands.(number): ...` (decrease if it takes a long time to kick the player, or increase if causes false positives)

### Contact
There are a lot of ways to contact me, but here are the main ones:

1. [Matrix's official discord](https://discord.gg/Vq93vdj) - recommended

2. [The config's official discord](https://discord.gg/2ReynYN) - for update notifications or larger debates (lol).

### FAQ
1. **Why is the anti-killaura NPC spawned in the HitBox check?**

This check also checks if the player isn't using Angle cheats, and the NPC checks if the player can hit people behind the player. To prevent lag and false positives from happening with this, the NPC will be spawned only if the player's ping is lower than 185ms. If I'm right, this should make the killaura detection more strict.
