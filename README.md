# not-curseme
A fork (i think) of [curseme](https://git.sakamoto.pl/domi/curseme) but i changed some stuff cause i couldnt be bothered to email the dev

stuff you need: 

- p7zip
- jq
- bash
- curl
- java (well, duh)
- busybox OR gnu coreutils 

its pretty much any functional and working linux computer (macos might work too but idk didnt try, might test it when i have time)

works exactly the same: 

1. Download a ZIP file from curseforge. This is hidden - curse really wants you to use their application. Go to Files -> Main File -> (click on the name) -> `Download` (NOT `Install`)
2. Clone this repository
3. Get an API key, and place it into the `token` file. You can do this legimately (I'll be here all day, we have time) or use `./getToken.sh` which extracts them from the CurseForge Client
4. Launch `parsePack.sh`; e.g. `./parsePack.sh "Above and Beyond-1.3.zip"`. This will download all of the mods.
5. If everything succeeds, a forge installer should pop up after a while. ~~Fabric support is not available at this time~~ Fabric works too (hopefully), and it should download that maybe.
6. Backup your `~/.minecraft` directory (super important './install.sh' will delet stuff there so you might want to do that)
7. Launch `./install.sh`
8. Profit..?


if you want to put it in the default launcher mc launcher cause you think being able to have multiple packs at once is cool, you should stop at step 4. and use my [guide](https://github.com/yav12/stuff/blob/main/howto-defaultmc.md).

:>
