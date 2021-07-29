## Hola amiguitos

This is my attempt to fix up and add a little crDroid customization flavor back into the sdm845 kernel tree for OnePlus 6 & 6T (enchilada & fajita).

Rebased on the official lineage-17.1 branch from LineageOS as of the end ofOctober 2021, with some extra goodies added in like clang 12 & 13 support, multiple vibration type support, wireguard support, and battery-idle-mode-enabled charging switches, among others.

I also added my DC Dimming (among other things) commit. more relying on bizarro-world "main_display" symlinks that make the SDM845 kernel different than all the other, newer OnePlus devices, making it difficult to implement features like DC dimming, etc. in the device tree.

If anyone is still reading, hi. You're pretty cool. There has been a lot of work on this, and most of it will never be visible, but at least you know I spent many hours of blood, sweat, and hair-pulling trying to test & fix things; and then most of that work was repeatedly rendered moot, but some of it at least has been getting picked up & cleaned up by smarter people than me and hopefully everyone will get to benefit from it.

Not TOO shabby for someone who doesn't actually know any c/c++/java. :D
