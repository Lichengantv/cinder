# Cinder

Control panel for a Paper Minecraft server on Windows 11, plus the Nokia Beacon 2 port-forward steps.

The site in `docs/` is static. It runs in the browser. It does not start Java. The world runs on your PC from `CinderHost.exe`.

## Use it on GitHub Pages

1. This repository must stay **public**.
2. On GitHub, open **Settings**.
3. In the left sidebar, open **Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5. Set the branch to **main** and the folder to **/docs**.
6. Click **Save**.
7. Wait about a minute. The site is https://lichengantv.github.io/cinder/

If the Windows download button on that site fails, upload `CinderHost.exe` into the `docs` folder (Add file, Upload files). The button looks for that exact name next to `index.html`.

## Run the Minecraft server

1. On the Windows 11 PC, install **Temurin 21** from https://adoptium.net. Tick **Add to PATH**.
2. Put `CinderHost.exe` in any folder. If you changed the MOTD, port, memory, scoreboard, or ranks in the panel, also put `cinder.json` in that same folder.
3. Double-click `CinderHost.exe`.
4. The first time, type `AGREE` to accept the Minecraft EULA.
5. When the console says `Done`, type `op YourMinecraftName`.
6. People in the house connect to the PC's IPv4 address. People outside the house need the Beacon forward (TCP 25565) and your public address. The steps are in the site under **Network**, and in `CinderHost\READ-ME.txt` after the first launch.
7. Stop the world by typing `stop` in that window.

Do not forward port 25575.
