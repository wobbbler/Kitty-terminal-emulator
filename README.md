# Kitty-terminal-emulator
## Установка

```bash
curl -L https://sw.kovidgoyal.net/kitty/installer.sh | sh /dev/stdin
```

## Настройка
Конфиг должен быть в `~/.config/kitty`

## Зависимости 

```bash
sudo apt update
sudo apt install -y fzf fonts-jetbrains-mono
fc-cache -f
```

## Ссылки 

Для запуска из терминала:
```bash
ln -sf ~/.local/kitty.app/bin/kitty ~/.local/bin/
ln -sf ~/.local/kitty.app/bin/kitten ~/.local/bin/
```

Для интеграции с системой:
```bash
cp ~/.local/kitty.app/share/applications/kitty.desktop ~/.local/share/applications/
sed -i "s|Exec=kitty|Exec=$HOME/.local/kitty.app/bin/kitty|g" ~/.local/share/applications/kitty.desktop
```
# Kitty-terminal-emulator
