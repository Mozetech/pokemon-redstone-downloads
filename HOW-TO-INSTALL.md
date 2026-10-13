# Pokémon Redstone 1.0.0: how to install

Minecraft Steve with survival in FireRed's Kanto, the Nether and The End. These downloads are the same game as
https://pokemon-redstone.pages.dev, packed as an app so it plays offline. Pick the file for your device:

| Device | File |
|---|---|
| Mac with Apple Silicon (M1 or newer) | `PokemonRedstone-1.0.0-mac-arm64.zip` |
| Mac with an Intel chip | `PokemonRedstone-1.0.0-mac-x64.zip` |
| Windows 10 or 11 (64-bit) | `PokemonRedstone-1.0.0-win-x64.zip` |
| Linux (64-bit x86, with a desktop) | `PokemonRedstone-1.0.0-linux-x64.tar.gz` |
| Android 7 or newer, including Retroid, AYN and Anbernic handhelds | `PokemonRedstone-1.0.0-android.apk` |

Not sure which Mac you have? Apple menu > About This Mac: "Chip: Apple M..." is Apple Silicon, "Processor: Intel" is Intel.

## macOS (13 Ventura or newer)

1. Unzip the file (double-click it; Safari may already have done this).
2. Drag **Pokemon Redstone** into your **Applications** folder.
3. Open it. The app is not notarized by Apple, so the first launch is blocked. To allow it once:
   - **Any macOS version:** try to open the app, close the warning, then open **System Settings > Privacy & Security**,
     scroll down to the note about "Pokemon Redstone" and click **Open Anyway**. Confirm with your password.
   - **macOS 13 or 14 only:** right-click (or Control-click) the app, choose **Open**, then **Open** again.

After that it opens normally. Fullscreen: Control+Command+F, or the green button at the top left of the window.

## Windows

1. Right-click the zip and choose **Extract All**. The game does not run from inside the zip.
2. Open the extracted **PokemonRedstone** folder and run **PokemonRedstone.exe**.
3. The app is not signed, so SmartScreen may say "Windows protected your PC". Click **More info**, then **Run anyway**.

Fullscreen: F11 or Alt+Enter.

## Linux

1. Unpack it: `tar -xzf PokemonRedstone-1.0.0-linux-x64.tar.gz` (this makes a folder named `PokemonRedstone`).
2. Run the launcher: `cd PokemonRedstone && ./PokemonRedstone`
3. If your file manager unpacked it without the run permission, fix that once:
   `chmod +x PokemonRedstone pokemon-redstone chrome_crashpad_handler`

This build is a folder with a launcher, not an AppImage. On systems that block Chromium's sandbox (Ubuntu 23.10 and
newer), the launcher turns the sandbox off for this app only. Fullscreen: F11 or Alt+Enter.

## Android

The app is not on Google Play. You install the APK file yourself:

1. Download `PokemonRedstone-1.0.0-android.apk` on the phone or handheld and open it (from the download notification
   or the Files app).
2. Android asks you to allow installs from this source (your browser or file manager). Tap **Settings**, turn on
   **Allow from this source**, go back and tap **Install**.
3. If Google Play Protect warns about an unknown app, tap **More details**, then **Install anyway**.

The game runs in landscape, fullscreen. The Back button is the game's B button, so it never closes the game: use Home
or Recents to leave. If the app says to update Android System WebView, update it (and Google Chrome) in the Play Store.

To update later, install the new APK over the old one. Do not uninstall first: uninstalling deletes your worlds.

## Controls

Keyboard: arrows or WASD move, Z is A, X is B, Space jumps, E opens the inventory, Q drops, C and V change the hotbar
slot, Shift sprints, J opens the map, Enter is START. On a touch screen the on-screen pad appears.

### Controllers

Plug in or pair the controller, then press any button once so the game sees it. A note confirms which button is A.
Built-in handheld controls work the same way. Using a controller hides the touch pad; touching the screen brings it back.

| Xbox / PlayStation | Nintendo | In the game |
|---|---|---|
| D-pad or left stick | D-pad or left stick | Move, and move the cursor in menus |
| A / Cross (bottom) | A (right) | A: mine, attack, talk, confirm |
| B / Circle (right) | B (bottom) | B: use, place, eat, go back |
| X / Square (left) | Y (left) | Jump |
| Y / Triangle (top) | X (top) | Inventory (also closes Minecraft screens) |
| LB / RB | L / R | Previous / next hotbar slot |
| LT | ZL | Drop one item |
| RT, or click the left stick | ZR, or click the left stick | Sprint (hold) |
| Select / Back / View | Minus | Full map |
| Start / Menu / Options | Plus | START menu |

**Swapping A and B.** Nintendo pads are recognised and get A on the right. Handhelds and other pads start with A on
the bottom. To swap, hold **SELECT and START together for 2 seconds** (Minus and Plus on a Nintendo pad); a note
confirms it. In generated worlds you can also use START > OPTION > A BUTTON. The game remembers your choice.

## Saves

Your worlds are saved on your device, separately from the website's saves: worlds made on the website do not appear
in the app, and the other way round.

- macOS: `~/Library/Application Support/Pokemon Redstone`
- Windows: `%APPDATA%\Pokemon Redstone`
- Linux: `~/.config/Pokemon Redstone`
- Android: inside the app (uninstalling the app deletes them)

## Co-op

Co-op needs the internet; everything else plays offline. App players and website players share the same rooms: one
player picks START > CO-OP > HOST and gets a five-letter code, and up to three others, on the app or on the website,
pick JOIN and type it in. Without a connection, HOST says "Co-op needs the internet. Check your connection." and the
game carries on.

## Checking the downloads

`SHA256SUMS.txt` lists each file's SHA-256. On macOS or Linux run `shasum -a 256 -c SHA256SUMS.txt` in the download
folder; on Windows run `certutil -hashfile PokemonRedstone-1.0.0-win-x64.zip SHA256` and compare.

## Fan notice

Unofficial fan project. Free: no ads, no donations. Not affiliated with Nintendo, Game Freak, The Pokémon Company,
Mojang or Microsoft.
