# Dependencies

## Wayland

### Chrome, Electron и т.п.

В зависимости от места установки `~/.local/share/applications/`
или `/usr/share/applications/` открыть файл *.desktop .

Нужно добавить флагу в кажду строку с `Exec`:
```text
Exec=/usr/bin/google-chrome-stable --enable-features=UseOzonePlatform --ozone-platform=wayland %U
```

Проверка для Chrome:
```
chrome://flags
chrome://version
chrome://gpu
```

## Tools

### helix

- [Docs1]https://helix-editor.com/
- [Docs2]https://helix-editor.vercel.app/
- [Src](https://github.com/helix-editor/helix)

```bash
snap install --classic helix
hx ~/.config/helix/config.toml
hx ~/.config/helix/languages.toml
```

### keyd

-[Src](https://github.com/rvaiya/keyd)

До ubuntu 25.04

```bash
git clone https://github.com/rvaiya/keyd
cd keyd
make && sudo make install
sudo systemctl enable --now keyd
```

С ubuntu 25.04

```bash
sudo apt install keyd
```

### ripgrep

```bash
sudo apt-get install ripgrep
```

### zellij

- [Docs](https://zellij.dev)
- [Src](https://github.com/zellij-org/zellij/)

```bash
curl -L https://github.com/zellij-org/zellij/releases/download/v0.44.3/zellij-x86_64-unknown-linux-musl.tar.gz -o /tmp/zellij.tar.gz
tar -xzf /tmp/zellij.tar.gz -C /tmp
sudo mv /tmp/zellij /usr/local/bin/
zellij --version
mkdir ~/.config/zellij
zellij setup --dump-config > ~/.config/zellij/config.kdl
```

### yazi

- [Docs](https://yazi-rs.github.io)
- [Src](https://github.com/sxyazi/yazi)

```bash
sudo snap install yazi --classic
```


### bat
### glow
### delta
### mergiraf
### dprint

## lsp

### sql

postgres-language-server
https://pg-language-server.com/latest/

### go
https://go.dev/doc/install
https://go.dev/gopls/
https://github.com/go-delve/delve
https://github.com/nametake/golangci-lint-langserver

### markdown

https://oxide.md/
https://github.com/Feel-ix-343/markdown-oxide