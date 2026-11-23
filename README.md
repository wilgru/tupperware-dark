# Tupperware Dark

A dark theme for Zed and Ghostty inspired by the Tupperware brand palette. The Zed theme started from Ayu Dark.

## Zed

Copy [`zed/tupperware-dark.json`](zed/tupperware-dark.json) to `~/.config/zed/themes/`, then select **Tupperware Dark** in the theme picker.

### Optional: purple Swift attributes

The Swift extension normally highlights `@State` and other attributes as variables. The [Swift query patch](zed/swift-attributes.patch) gives the `@` and attribute name their own highlight so the theme can color them purple without recoloring ordinary variables or attribute arguments.

From this repository on macOS, check the patch and apply it if the check passes:

```sh
swift_extension="$HOME/Library/Application Support/Zed/extensions/installed/swift"
git -C "$swift_extension" apply --check "$PWD/zed/swift-attributes.patch" &&
  git -C "$swift_extension" apply "$PWD/zed/swift-attributes.patch"
```

Restart Zed afterward. Skip this step if the patch is already applied. Swift extension updates may overwrite the local change or change the query enough to prevent the patch from applying.

## Ghostty

Copy [`ghostty/Tupperware Dark`](ghostty/Tupperware%20Dark) to `~/.config/ghostty/themes/`, then set `theme = Tupperware Dark` in your Ghostty config and reload it.
