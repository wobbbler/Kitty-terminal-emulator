# Kitty Terminal Emulator

## Dependencies
- `fzf`
- `fonts-jetbrains-mono`

**For Ubuntu:**
```bash
sudo apt update && sudo apt install -y fzf fonts-jetbrains-mono
fc-cache -f
```

---

## Installation
```bash
curl -L https://sw.kovidgoyal.net/kitty/installer.sh | sh /dev/stdin
```

---

## Configuration
**Path:** `~/.config/kitty`

---

## Links

**Terminal launcher:**
```bash
ln -sf ~/.local/kitty.app/bin/kitty ~/.local/bin/
ln -sf ~/.local/kitty.app/bin/kitten ~/.local/bin/
```

**System integration:**
```bash
cp ~/.local/kitty.app/share/applications/kitty.desktop ~/.local/share/applications/
sed -i "s|Exec=kitty|Exec=$HOME/.local/kitty.app/bin/kitty|g" ~/.local/share/applications/kitty.desktop
```
