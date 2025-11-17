# fuzzy-pacman (fpm)

fpm is a fuzzy and interactive wrapper around pacman using **skim (sk)**.  
It provides fast package management via fuzzy menus with real-time previews and multi-selection.

---

# Features

- Fuzzy install and remove packages
- Fuzzy search in repositories
- Inspect installed packages
- List package files
- Manage orphan dependencies
- Explore systemd services interactively
- Search which package owns a file
- Clean pacman cache via fuzzy interface
- Browse packages by repository
- Fully keyboard-driven and fast

---

# Installation on Arch Linux

## AUR (recommended)

Using **pacman** with an AUR helper:

```bash
pacman -S fuzzy-pacman
```

Using **yay**:

```bash
yay -S fuzzy-pacman
```

Using **paru**:

```bash
paru -S fuzzy-pacman
```

## Manual installation (makepkg)

Clone the repository:

```bash
git clone https://github.com/brunos3d/fuzzy-pacman.git
cd fuzzy-pacman
```

Build and install:

```bash
makepkg -si
```

## Manual installation (without makepkg)

```bash
sudo install -Dm755 fpm /usr/bin/fpm
```

---

# Available commands

Install packages:

```bash
fpm - fuzzy pacman wrapper

Commands:
  sync      Sync pacman databases (pacman -Sy)
  add       Install packages
  rm        Remove packages
  search    Search repository
  info      Inspect installed packages
  update    Show updates
  files     List package files
  orphans   Remove orphan dependencies
  file      Repo file provider lookup
  own       Installed file owner lookup
  repo      Browse repositories
  svc       Browse systemd services
  cache     Clean pacman cache
  bulk      Bulk menu
  help      Show help
```

---

# Dependencies

- pacman
- skim (sk)
- systemd (for svc subcommand)

---

# License

MIT License
