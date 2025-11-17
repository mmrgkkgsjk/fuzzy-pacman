# fuzzy-pacman (fpm)

fpm is a fuzzy and interactive wrapper around pacman using **skim (sk)**.  
It provides fast package management via fuzzy menus with real-time previews and multi-selection.

All functionality is grouped under a single command:

```
fpm <subcommand>
```

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

# Subcommands

### Install packages

```
fpm add
```

### Remove installed packages

```
fpm rm
```

### Search repository packages

```
fpm search
```

### Show info about installed packages

```
fpm info
```

### List files installed by a package

```
fpm files
```

### Remove orphan dependencies

```
fpm orphans
```

### Show available updates

```
fpm upd
```

### Search which package provides a file (from repos)

```
fpm file
```

### Search which package owns a system file (installed)

```
fpm own
```

### Explore packages by repo (core, extra, multilib)

```
fpm repo
```

### Fuzzy browse systemd services

```
fpm svc
```

### Clean pacman cache interactively

```
fpm cache
```

---

# Dependencies

- pacman
- skim (sk)
- systemd (for svc subcommand)

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

# Usage examples

Install packages:

```bash
fpm add
```

Remove packages:

```bash
fpm rm
```

Search repository packages:

```bash
fpm search
```

Browse systemd services:

```bash
fpm svc
```

Clean the pacman cache:

```bash
fpm cache
```

---

# License

MIT License
