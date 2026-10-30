# Window Rescue

Bring windows that went off screen back.

In the Add-ons window (the Add-ons button in the menu), under Map & Windows: a "Bring all windows on screen" button that moves any window sitting partly or fully off screen back into view.

An add-on for [ROSE Mod Launcher](https://github.com/Zurnny/Rose_Mod_Launcher), for the game's default UI and the Steampunk UI theme. Without the launcher, copy the `Data` folder from `files` into your ROSE Online folder.

## Install
1. Download this repo (Code > Download ZIP) and open it.
2. Copy the **Window Rescue** folder into `Launcher Mods` in your ROSE Online folder.
3. Open the launcher, press **Mods**, tick **Window Rescue**, and restart the game.

It updates itself from this repo whenever the launcher opens.

## Works with the other add-ons
Every add-on works on its own, and any mix of them works together. Add-ons
that change the same window (the Add-ons window, the menu, the HUD, the party
and group windows)
carry the very same copy of that file, and each part only runs while its own
add-on is installed: each add-on puts a small marker file in
`Data/ui/sp_addons/`, which the launcher removes again with the add-on.
In the **Add-ons** window (the Add-ons button in the menu) each installed
add-on adds its own line or settings to its section (Combat, HUD, Party &
Social, Items & Crafting, Chat, Map & Windows), one
under the other, in the order they are listed there.

## Default UI or Steampunk
Each window it changes holds both looks: the game's own and the [Steampunk UI](https://github.com/Zurnny/SteamPunk) theme's. When the window opens it checks whether Steampunk is installed (`styles/steampunk.css`) and uses that look, so it works with either one, with or without the launcher. With Steampunk, the Steampunk theme's own features stay on too.

The switches are saved in `sp_addons.txt` in the ROSE Online folder. The Ice UI
theme uses the same file; both keep each other's settings.

## Files it changes
- `Data/ui/themes/rose/game/menu.html`
- `Data/ui/themes/rose/game/options_bgfx.html`
- `Data/ui/themes/rose/game/sp_addons_window.html`
- `Data/ui/themes/rose/styles/sp_addons_steampunk.css` (Steampunk look, shared by the add-ons)
- `Data/ui/themes/rose/styles/sp_addons_steampunk_sprites.css` (Steampunk look, shared by the add-ons)
- `Data/ui/themes/rose/imgs/sp_addons_menu.dds` (the Add-ons button, default UI)
- `Data/ui/sp_addons/window_rescue.txt` (marker)

Turning it off in the launcher puts the game's own files back.
