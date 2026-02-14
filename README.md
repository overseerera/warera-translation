# War Era Translations

This repository contains the translation files for [War Era](https://warera.com). Community contributions are welcome!

## Structure

Each locale has its own directory with a `messages.po` file:

```
en/messages.po   # English (source locale)
es/messages.po   # Spanish
fr/messages.po   # French
it/messages.po   # Italian
lv/messages.po   # Latvian
pl/messages.po   # Polish
pt/messages.po   # Portuguese
ro/messages.po   # Romanian
sr/messages.po   # Serbian
tr/messages.po   # Turkish
uk/messages.po   # Ukrainian
```

## How to Contribute

1. **Fork** this repository
2. **Edit** the `.po` file for the language you want to translate
3. **Submit a Pull Request**

### Editing `.po` files

Each `.po` file contains entries like this:

```po
#: src/components/SomeComponent.tsx:42
msgid "Hello, world!"
msgstr ""
```

- `msgid` is the original English string (do **not** modify this)
- `msgstr` is the translation — fill this in for your language
- Lines starting with `#:` are source references (do not modify)
- Lines starting with `#.` are developer comments providing context

An empty `msgstr ""` means the string is untranslated and will fall back to English.

### Tools

You can edit `.po` files with:
- Any text editor
- [Poedit](https://poedit.net/) — a dedicated `.po` file editor with a nice UI
- [Weblate](https://weblate.org/) or similar online tools

### Placeholders

Some strings contain placeholders like `{0}`, `{username}`, or XML-like tags `<0>...</0>`. Make sure to **keep all placeholders intact** in your translation:

```po
msgid "Welcome, {0}!"
msgstr "Bienvenue, {0} !"
```

```po
msgid "Click <0>here</0> to continue"
msgstr "Cliquez <0>ici</0> pour continuer"
```

## Guidelines

- Do not translate the `en/messages.po` file (it is the source locale, auto-generated)
- Keep the tone consistent with the game's style
- If you're unsure about a translation, leave a comment on your PR
- Test your changes if possible by running the game locally

## Adding a New Language

If you'd like to add support for a new language, please open an issue first so we can discuss it.

## License

These translation files are part of the War Era project.
