# Windows 7 Theme for Cinnamon 22.x

<img width="1920" height="1080" alt="Screenshot from 2026-04-08 07-18-43" src="https://github.com/user-attachments/assets/5baf4c9c-254f-4fba-ad2b-d17fcc0b7188" />

This repository is a pragmatic and somewhat dirty compatibility fix (by me and GPT) for the classic B00merang Windows 7 theme on modern Cinnamon 6.x / Linux Mint 22.x / GTK3 / GTK4 code.

The point of this repo is to let people use the theme again in the current Cinnamon without obvious visual problems, broken controls, unreadable text, or awkward spacing. It is **not** intended to be a perfect visual clone of W7.

My changes include adjustments for things like:

- Cinnamon Shell spacing and dialog styling
- Progress bars and selected-row progress rendering
- Better contrast for light popups and secondary text
- Headerbar and title button fixes in GTK3 and GTK4
- End-session dialog improvements
- Sound applet overlay readability
- A Windows 7-like corner bar / “Show desktop” strip
- Small Nemo and general usability refinements

## Supported platforms

- Cinnamon 6.6+

I have no idea what this theme does to other DEs.

## Installation

This theme is meant to be installed following the same overall process shown in the [OMG! Ubuntu guide for making Linux Mint look like Windows 7](https://www.omgubuntu.co.uk/2020/01/make-linux-mint-look-like-windows-7). That guide installs the original theme pack, icon pack, and related desktop tweaks.

### 1. Install the fixed Windows 7 theme pack

Download the [fixed Windows 7 theme pack](https://github.com/Xalalau/Windows-7-theme-cinnamon/archive/refs/heads/master.zip), extract it, and copy the extracted folder to your `~/.themes` directory. Then open Mint’s **Themes** settings and apply it to applications and desktop.

### 2. Install an icon set

Download the [fixed Windows 7 icon set](https://github.com/Xalalau/Windows-7-Icons-Cinnamon/archive/refs/heads/master.zip) and extract it into your `~/.icons` directory, then select it in Mint’s **Themes** settings.

If you prefer, the theme mixes very well with [Windows 11 icons](https://github.com/yeyushengfan258/Win11-icon-theme).

But my personal favorite is [Papirus](https://community.linuxmint.com/software/view/papirus-icon-theme).

### 3. Use a light theme variant

This is also important.

Use **light themes** and light theme combinations wherever possible. Dark variants tend to introduce visual inconsistencies, unreadable text, or mismatched assets. GIMP is a good example of a problematic application because it tends to come in dark mode (Flatpak) and immediately shows style errors.

If you want the theme to look correct, stick to light setups.

### 4. Optional finishing touches

#### Try out a new menu

I support both **[CinnVIIStarkMenu](https://cinnamon-spices.linuxmint.com/applets/view/281)** and **[Cinnamenu](https://cinnamon-spices.linuxmint.com/applets/view/322)**.

E.g. In Cinnamon:

- right-click the panel
- open **Applets**
- go to **Download**
- search for **Start Menu**
- install **CinnVIIStarkMenu**
- add it to the panel

#### Change the wallpaper

Set an [appropriate Windows 7 wallpaper](https://github.com/maxik34/Project_7/tree/main/Wallpapers/PNG), which helps complete the overall look.

Download from here for a bonus: https://imgur.com/a/4IaTbVZ

#### Install Microsoft fonts

For an even better experience, you may also want to install and use the Microsoft core fonts package.

Look for either `ttf-mscorefonts-installer` or `mscore` in the **Software Manager**.

After installing it, you can set your system font to **Segoe UI** for a closer Windows 7 look (Suggested by vaestgotaspit).

Another benefit is that these fonts will also become available in Office applications and some games, which can improve overall compatibility.

#### Use Drawer

Another applet worth recommending is [Drawer (show/hide applets)](https://cinnamon-spices.linuxmint.com/applets/view/169). It helps keep the panel cleaner by letting you hide a group of applets and show them again with a mouse iteraction.

This fits the Windows 7 vibe well, as on Windows it's common to keep tray icons collapsed instead of showing everything all the time.

#### Use `xscreensaver`

I recommend using **xscreensaver**.

Features like this belong to the Windows 7 era. It's not required, but it matches the spirit of the setup better.

#### Remove Windows logo

If you are not a fan of Microsoft but do like Windows 7 style, I assume you did not install the official background and want to remove the Start Menu logo. To do that, run the command below:

```bash
sed -i '/#panelLeft \.applet-box:first-child {/,/^}/d; /#panelLeft \.applet-box:first-child:hover {/,/^}/d; /#panelLeft \.applet-box:first-child:active {/,/^}/d' ~/.themes/Windows-7-Theme-Cinnamon/cinnamon/cinnamon.css && nohup cinnamon --replace >/dev/null 2>&1 & disown
```

If you want to re-enable the Start Menu logo, reinstall the theme.

## Scope and maintenance

This repository is just a **rough** fix so people can use the theme again.

I am **not** planning to actively maintain this project.

That means:

- no long-term maintenance commitment
- no promise of future compatibility updates
- no active feature development
- no PR review workflow
- no effort toward polishing this into a “properly maintained” theme fork

This repo exists because I wanted a working repair, not a new full-time project.

## Known issues

- Nemo's file preview uses a separate window that does not integrate cleanly with the active theme. Any attempt to force white text there, such as ``window.background label { color: #ffffff; }``, ends up affecting unrelated parts of the OS as well. The only clean way to do it globally would be to explicitly redefine the exact color of labels across the entire system, and I'm not going to do that.

## More media

<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-15-51" src="https://github.com/user-attachments/assets/be054488-b189-474c-8b56-62f1e00cdd81" />
<img width="1920" height="1080" alt="Screenshot from 2026-04-08 07-25-43" src="https://github.com/user-attachments/assets/4139203d-bbaa-42df-8c6b-1b2c8395f0d6" />
<img width="1920" height="1080" alt="Screenshot from 2026-04-08 07-19-09" src="https://github.com/user-attachments/assets/b54e3769-6aaf-4dd8-ba66-34d06340f797" />
<img width="1920" height="1080" alt="Screenshot from 2026-04-08 07-20-06" src="https://github.com/user-attachments/assets/034edf25-387d-495b-a0cf-4071a3a15886" />
<img width="1920" height="1080" alt="Screenshot from 2026-04-08 07-24-30" src="https://github.com/user-attachments/assets/bc93bf1f-bfbe-42c3-b8e0-149b4749f3e2" />
<img width="1920" height="1080" alt="Screenshot from 2026-04-08 07-22-14" src="https://github.com/user-attachments/assets/c9b4c7d8-b3c7-4993-94da-c41ed7fb6a9d" />
<img width="1920" height="1080" alt="Screenshot from 2026-04-08 07-21-32" src="https://github.com/user-attachments/assets/c6b163e3-8a2d-439c-9137-7766a4f275df" />
<img width="1920" height="1080" alt="Screenshot from 2026-04-08 14-03-58" src="https://github.com/user-attachments/assets/01b4bda8-d312-422e-a1c5-86baed4eba11" />

