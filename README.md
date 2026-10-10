# CCSoM — All of Create Aeronautics

Auto-updating modpack for the **Captain Codiene Squad of Misfitz** server.
Minecraft 1.21.1 · NeoForge 21.1.250 · distributed with [packwiz](https://packwiz.infra.link/).

Every time you press **Play**, the pack checks this repository and downloads only what changed.
You never have to reinstall the pack by hand.

## Install (one time)

1. Install **[Prism Launcher](https://prismlauncher.org/)** and log in with your Microsoft account.
2. Download **[CCSoM-Prism-Instance.zip](https://github.com/Shadxku/ccsom-modpack/raw/main/prism/CCSoM-Prism-Instance.zip)**.
3. In Prism: **Add Instance → Import → Browse**, pick the zip, and click **OK**.
4. Select the new instance and press **Launch**.
   - The first launch downloads about 900 MB of mods and configs. A small updater window shows the progress.
   - The instance is set to 8 GB of memory. If your PC has less than 16 GB of RAM, lower it in
     **Edit → Settings → Java**.
5. Join the server from **Multiplayer**.

## Updating

Nothing to do. Just launch the instance: new or changed mods are downloaded automatically before
the game starts. See [CHANGELOG.md](CHANGELOG.md) for what changed.

Your `options.txt` (keybinds, video settings) is only installed the first time, so updates never
overwrite your settings.

## Troubleshooting

- **"Mod mismatch" / can't join the server:** close the game and launch again so the updater runs.
- **Updater window shows an error:** check your internet connection and try again. If it keeps
  failing, tell Shadxku.
- **Want to use another launcher?** Only launchers that support pre-launch commands (Prism, MultiMC)
  can auto-update. Otherwise ask for the latest zip.

## For the pack maintainer

- `pack.toml` / `index.toml` are the packwiz files. `index.toml` lists every file with a SHA-256 hash.
- Mod jars are stored in `mods/`, configs in `config/`, etc. — exactly as in the game folder.
- After changing any file, regenerate `index.toml` and update the hash in `pack.toml`, then push.
