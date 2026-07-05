# vs-code-settings

My VS Code settings, style config, and extension list.

## Contents

- `settings.json` — VS Code user settings (theme, glass/vibrancy, editor)
- `vibrancy/nvim-gruvbox.css` — custom CSS for `illixion.vscode-vibrancy-continued`
- `extensions.txt` — installed extensions

## Restore

```sh
DEST="$HOME/Library/Application Support/Code/User"   # macOS
cp settings.json "$DEST/settings.json"
mkdir -p "$DEST/vibrancy" && cp vibrancy/nvim-gruvbox.css "$DEST/vibrancy/"
cat extensions.txt | xargs -L1 code --install-extension
```
