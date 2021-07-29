## Hola amiguitos

This is my attempt to fix up and add a little crDroid customization flavor back into the sdm845 kernel tree for OnePlus 6 & 6T (enchilada & fajita).

Rebased on the official lineage-20 branch from LineageOS as of January 2023, plus merged 4.9 LTS kernel security updates from AOSP thanks to BananaFunction, with some extra goodies added in like clang 12+ support, wireguard support, vibration control, digital audio gain controls, OOS panel color modes, zstd support for zram, and so on. Fancy! Much thanks to mcdachpappe for the excellent MCD kernel; I'm mostly using his curated commits for extra features since they're a lot cleaner than my previous hodgepodge stack of cherry-picks.

If anyone is actually reading this, hi. You're pretty cool. There has been a lot of work on this, and most of it will never be visible, but at least you know I spent many hours of blood, sweat, and hair-pulling trying to test & fix things; and then most of that work was repeatedly rendered moot, but some of it at least has been getting picked up & cleaned up by smarter people than me and hopefully everyone will get to benefit from it.

Not TOO shabby for someone who doesn't actually know any c/c++/java. :D

Currently includes some temp hax to fix compiling under clang 16. If you're using clang-14 or older, you might be better off dropping the last two commits.
