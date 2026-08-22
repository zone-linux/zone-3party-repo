# zone-3party-repo

Third-party (AUR) binary package repository for Zone Linux.

Served at: `https://zone-linux.github.io/zone-3party-repo/x86_64/`

## Contents

Packages built from AUR sources listed in `zone-pkgbuild/3rdparty_pkgbuild/aurpackages`:

`ani-cli-git`, `cava`, `ckbcomp`, `grub2-theme-preview`, `kvantum-theme-qogir-git`,
`minecraft-launcher`, `mkinitcpio-openswap`, `nerd-fonts-jetbrains-mono`,
`oh-my-zsh-git`, `paru-bin`, `qogir-gtk-theme-git`, `qogir-icon-theme-git`,
`shell-color-scripts`, `tty-clock-git`, `ulauncher`, `unimatrix-git`,
`xfce-polkit`, `ytfzf-git`

## Updating

Clone the latest AUR PKGBUILDs on a Linux host using `zone-pkgbuild/3rdparty_pkgbuild/get-pkgs.sh`,
build them, and run `zone-pkgbuild/upd-3party.sh` to publish.

## Note

The `nerd-fonts-jetbrains-mono` package in this repo is at version 2.1.0-3 (2022).
The Arch official repos now carry `ttf-jetbrains-mono-nerd` — the ISO `packages.x86_64`
has been updated to use the official package instead of this custom one.
