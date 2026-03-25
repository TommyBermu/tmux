# Mi config de tmux (Arch Linux)

Config personal de tmux para productividad:
- Prefijo: Ctrl+s
- Navegacion entre paneles estilo vim
- Plugins con TPM
- Tema Catppuccin en la barra de estado

El archivo principal es .tmux.conf.

## Requisitos

En Arch instala lo basico con:

```bash
sudo pacman -Syu tmux git curl wl-clipboard
```

Opcional pero recomendado:
- Una Nerd Font (ej: JetBrainsMono Nerd Font)
- Terminal con buen soporte de glifos (Kitty, Alacritty, etc.)

## Instalacion rapida

1. Clonar este repo:

```bash
git clone https://github.com/TommyBermu/tmux.git ~/.config/tmux
```

2. Instalar TPM:

```bash
git clone https://github.com/tmux-plugins/tpm ~/.config/tmux/plugins/tpm
```

3. Abrir tmux e instalar plugins:
- Presiona Ctrl+s luego Shift+i

Tambien puedes hacerlo por comando:

```bash
~/.tmux/plugins/tpm/bin/install_plugins
```

4. Recargar config:

```bash
tmux source-file ~/.config/tmux/tmux.conf
```

## Plugins usados

- tmux-plugins/tpm
- tmux-plugins/tmux-sensible
- christoomey/vim-tmux-navigator
- tmux-plugins/tmux-resurrect
- tmux-plugins/tmux-continuum
- tmux-plugins/tmux-yank
- catppuccin/tmux

## Nota

Si no se ven bien los iconos en la barra, cambia la fuente de tu terminal a una Nerd Font.

