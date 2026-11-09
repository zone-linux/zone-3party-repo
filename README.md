# zone-3party-repo

Third-party (AUR) binary package repository for Zone Linux.

Served at: `https://zone-linux.github.io/zone-3party-repo/x86_64/`

## Contents

Packages built from the AUR sources listed in
`zone-pkgbuild/3rdparty_pkgbuild/aurpackages`:

`ani-cli-git`, `calamares`, `ckbcomp`, `grub2-theme-preview`,
`kvantum-theme-qogir-git`, `minecraft-launcher`, `mkinitcpio-openswap`,
`oh-my-zsh-git`, `paru-bin`, `qogir-gtk-theme-git`, `qogir-icon-theme-git`,
`tty-clock-git`, `ulauncher`, `unimatrix-git`, `xfce-polkit`, `ytfzf-git`

`cava`, `nerd-fonts-jetbrains-mono`, and `shell-color-scripts` were removed: `cava`
and the Nerd font are available from the official repositories, and
`shell-color-scripts` is no longer packaged.

## Updating

```bash
cd zone-pkgbuild
./3rdparty_pkgbuild/get-pkgs.sh          # clone or update AUR checkouts
./build.sh --3party --no-publish
./publish.sh --3party --prune --verify
./publish.sh --3party --commit           # commit locally; never pushes
```

Publishing keeps the newest staged package per name, drops `*-debug` packages,
removes orphans, retains two versions by default, and rebuilds the database so it
always references the newest on-disk archive.
