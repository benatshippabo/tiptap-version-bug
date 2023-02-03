# tiptap-version-bug

This repository reproduces the bug in the tiptap release process [where older release are overwritten.](https://github.com/ueberdosis/tiptap/issues/3692)

## Reproduction steps

```sh
yarn
```

Notice warnings about unmet dependencies on `@tiptap/pm `. However, `@tiptap/pm` was created after `@tiptap/react@2.0.0-beta.195`:

https://github.com/ueberdosis/tiptap/tree/v2.0.0-beta.195/packages

https://github.com/ueberdosis/tiptap/blob/v2.0.0-beta.195/packages/extension-bubble-menu/package.json
