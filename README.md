# Windows 7 Theme for Cinnamon 22.x

<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-07-30" src="https://github.com/user-attachments/assets/fb405725-4bb5-4638-bf5b-e271f906550f" />

This repository is a pragmatic and somewhat dirty compatibility fix (by me and GPT) for the classic B00merang Windows 7 theme on modern Cinnamon 6.x / Linux Mint 22.x / GTK3 / GTK4 code.

The point of this repo is to let people use the theme again in the current Cinnamon without obvious visual problems, broken controls, unreadable text, or awkward spacing. it is **not** intended to be a perfect visual clone of W7.

It includes adjustments for things like:

- Cinnamon Shell spacing and dialog styling
- Progress bars and selected-row progress rendering
- Better contrast for light popups and secondary text
- Headerbar and title button fixes in GTK3 and GTK4
- End-session dialog improvements
- Sound applet overlay readability
- A Windows 7-like corner bar / “Show desktop” strip
- Small Nemo and general usability refinements

A complete changelog is available below.

## Supported platforms

- Cinnamon 6.6+

I have no idea what this theme does to other DEs.

## Installation

This theme is meant to be installed following the same overall process shown in the [OMG! Ubuntu guide for making Linux Mint look like Windows 7](https://www.omgubuntu.co.uk/2020/01/make-linux-mint-look-like-windows-7). That guide installs the original theme pack, icon pack, and related desktop tweaks.

### 1. Install the fixed Windows 7 theme pack

Download the [fixed Windows 7 theme pack](https://github.com/Xalalau/Windows-7-theme-cinnamon/archive/refs/heads/master.zip), extract it, and copy the extracted folder to your `~/.themes` directory. Then open Mint’s **Themes** settings and apply it to applications and desktop.

### 2. Install the Windows 7 icon set

Download the [original Windows 7 icon set](https://github.com/B00merang-Artwork/Windows-7/archive/master.zip) and extract it into your `~/.icons` directory, then select it in Mint’s **Themes** settings.

### 3. Install **CinnVIIStarkMenu**

This is important.

The regular Cinnamon menu is **not supported well by this theme**. The setup depends on **CinnVIIStarkMenu** for a more appropriate Windows 7-style start menu experience. The same applet is also recommended in the original tutorial.

In Cinnamon:

- right-click the panel
- open **Applets**
- go to **Download**
- search for **Start Menu**
- install **CinnVIIStarkMenu**
- add it to the panel

### 4. Use a light theme variant

This is also important.

Use **light themes** and light theme combinations wherever possible. Dark variants tend to introduce visual inconsistencies, unreadable text, or mismatched assets. GIMP is a good example of a problematic application because it tends to come in dark mode (Flatpak) and immediately shows style errors.

If you want the theme to look correct, stick to light setups.

### 5. Optional finishing touches

#### Change the wallpaper

Set an [appropriate Windows 7 wallpaper](https://live.staticflickr.com/2685/4531929561_abf5cf4d71_o_d.jpg), which helps complete the overall look.

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

## More media

<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-15-51" src="https://github.com/user-attachments/assets/be054488-b189-474c-8b56-62f1e00cdd81" />
<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-14-55" src="https://github.com/user-attachments/assets/c194a4fa-41df-4e24-859f-d715d801b65b" />
<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-07-12" src="https://github.com/user-attachments/assets/51262b3f-d060-4c2f-80ac-f17343a335dc" />
<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-06-15" src="https://github.com/user-attachments/assets/c6a5fe7f-b801-4c1f-b864-0795758f320d" />
<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-05-24" src="https://github.com/user-attachments/assets/6abf26d2-e9b9-4bcf-8c2e-c05cccd1db10" />
<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-04-00" src="https://github.com/user-attachments/assets/2583a23f-3d34-4005-87df-54f04ecedbe0" />
<img width="1920" height="1080" alt="Captura de tela de 2026-04-06 22-02-48" src="https://github.com/user-attachments/assets/d9405dfb-7875-4370-8f20-e161a0a1badf" />

