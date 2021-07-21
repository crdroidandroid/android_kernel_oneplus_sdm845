## Hola amiguitos

We've gone kernel shopping again, and are using a slightly modified version of mcd kernel by mcdachpappe (https://github.com/mcdachpappe/),
specifically from their android_kernel_oneplus_sdm845-r2 repository (new arter97 base, release 5, custom-los-fod variant), with a few 
relevant tweaks to work with our device tree and for being built inline rather than as a prebuilt image or flashable zip installer.

WiFi performance should be at least as good as before, battery life better, and FOD far less buggy. It also seems to help with camera app
stability under Android 11 (for reasons that are beyond me). 

Since the stock LOS-based kernel from the previous couple releases won't ever be able to support both updated FOD commits and DC dimming,
due to how it has evolved (or not evolved, to be more accurate), we needed to jump ship, for all the reasons that were still true when we
used Illusion kernel back in March 2021. 

I was hoping that maybe the newer lineage-18.1 rebased kernel would serve us well, but it still 
has all the problems of rewritten display handling that still never incorporated updates from OOS Q kernel sources, and is now radically
different in alpha layer blending, FOD handling, and display mode handling than all of the kernels for newer OnePlus devices. In turn, 
this causes the sdm845-common device tree to also have to be entirely different; hampering any efforts to backport new features or make
things more consistent between OP 6-series, 7-series, 8-series, or now 9-series for ease of updating/sharing code. Oh well!
