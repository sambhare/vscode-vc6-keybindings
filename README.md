# Visual C++ 6.0 Keymap for Visual Studio Code

This extension ports several Visual C++ 6.0 keyboard shortcuts to Visual Studio Code. After installing the extension and restarting VS Code your favorite keyboard shortcuts from Visual C++ 6.0 are now available.

## What keyboard shortcuts are included?

You can see all the keyboard shortcuts in the extension's contribution list.

## Why aren't all the shortcuts included?

VS Code does not implement all of the commands that were available in Visual C++ 6.0. As a reference, <a href="https://msdn.microsoft.com/en-us/library/58feksch(v=vs.100).aspx">this page</a> lists all the shortcuts available in Visual C++ 6.0.

## Why does this install the Bookmarks extension?

Anonymous bookmarking via the F2 key was one of the most useful features of Visual C++ 6.0 and the [Bookmarks extension](https://marketplace.visualstudio.com/items?itemName=alefragnani.Bookmarks) combined with this keymap brings this functionality to VS Code.

## How do I contribute a keyboard shortcut?

It is very easy to make a PR.

1. Head over to the [GitHub repository](https://github.com/sambhare/vscode-vc6-keybindings).
2. Open [`package.json`](https://github.com/sambhare/vscode-vc6-keybindings/blob/master/package.json).
3. Add a JSON object to [`contributes.keybindings`](https://github.com/sambhare/vscode-vc6-keybindings/blob/master/package.json#L32) as seen below.
4. Open a pull request.

```json
{
    "mac": "<keyboard shortcut for mac>",
    "linux": "<keyboard shortcut for linux",
    "win": "<keyboard shortcut for windows",
    "key": "<default keyboard shortcut>",
    "command": "<name of the command in VS Code",
    "when": "<condition>"
}
```

You can read more about how to contribute keybindings in extensions in the [official documentation](http://code.visualstudio.com/docs/extensionAPI/extension-points#_contributeskeybindings).
