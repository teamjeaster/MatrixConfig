# MatrixConfig

> The optimized config for [Matrix Anticheat](https://matrix.rip/).

![Built with oxygen](https://badgen.net/badge/built%20with/oxygen/green) ![for matrix free](https://badgen.net/badge/for%20free%20matrix/4.7.10/green) ![and premium](https://badgen.net/badge/and%20premium%20matrix/4.8.0/green)

**Warning: The free version of Matrix isn't updated anymore - the last free version was 4.7.10. You should use `checks-free.yml` if you use it. Also, no, using the premium checks file won't get you premium features.** Premium user? See `checks-premium.yml`.

### Terms
You can use this for anything, and modify it if you want to, but just please don't say that it's entirely yours and no one else contributed to it.

### Important thing to remember
Don't assume that this config will be perfect for your server out of the box - each server is different, you should tweak the config for your own needs.

Also, remember that in most cases with Matrix, it's either get a big amount of false kicks or make the detection a little bit more lenient.

I can't make your anticheat kick people seconds after they turn on their hacks without causing false positives if I can't even access the code. This ain't NoCheatPlus.

### Recommended changes
1. `nofall.damage: true` -> `nofall.damage: false` (for minigame servers with fall damage disabled)

2. `block.noswing.enabled: false` -> `block.noswing.enabled: true` (if you don't use ViaVersion)

3. `hitbox.max-reach: 3.3` -> `hitbox.max_reach: 3.4` (if you have hitbox false positives **[makes hitbox detection more lenient!]**)