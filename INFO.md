# /tg/station Staff Minecraft Server

Hosted by lorwp

## Requirements

- Pack is All the Mods 9 0.2.37 Available [Here](https://www.curseforge.com/minecraft/modpacks/all-the-mods-9/files/5036838) with your Client of Choice
    - I personally use [Prismlauncher](https://prismlauncher.org/), i'd suggest using that or MultiMC
- Two additional mods required to connect are [Alex's Caves](https://www.curseforge.com/minecraft/mc-mods/alexs-caves/files/4952948) and it's Dependency [Citadel](https://www.curseforge.com/minecraft/mc-mods/citadel/files/4848887)

Once Setup you should have 410 Mods (as of Writing), and it'll look something like this in your mod list:
![image](https://hackmd.io/_uploads/rJ7PxWbta.png)

## Connecting

Connect to `mc.lorwp.cc`, default port.

### Whitelisting

Anyone who has connected at least once already before 17/1/2024 is already on the whitelist.

Anyone else, please contact lorwp or Isratosh in the tg discord to be whitelisted. Current and Retired tgstation staff only.

## Other Notes

- `/rtp` will teleport you to a random spot, if you need somewhere out of the way.
- Follow the questbook, it'll give you a lot of loot and give you things to aim for in this massive pack.

## Updating

When pinged about a update to ATM itself, assuming you're using Prismlauncher, just head to the settings of your instance, and click on `Curseforge`, and you'll see a screen like this:

![image](https://hackmd.io/_uploads/B1KSVXHY6.png)

Just select the required version at the dropdown, and click `Update Pack`.

If you're using any other launcher, i can't tell you how to update it, i'd suggest using the built in update function if there is one (Or worst case, just download the pack again entirely).

## Aikar's Flags

To improve performance, the following flags can be used to start minecraft, per [Aikar](https://aikar.co/2018/07/02/tuning-the-jvm-g1gc-garbage-collector-flags-for-minecraft/)

```bash
-XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=32M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -Dusing.aikars.flags=https://mcflags.emc.gs -Daikars.new.flags=true
```

## Changelog

- 17/1/2024: Updated ATM9 to 0.2.37, enforce whitelist
