# Dependencies

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