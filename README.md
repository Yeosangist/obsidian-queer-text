# Queer Flag Highlighter

An Obsidian plugin that colours queer-related words with their associated pride flag colours.

## Based on the Web Userscript

This plugin is an Obsidian port of the [Queer Flag Highlighter userscript](https://github.com/Yeosangist/queer-flag-text), which highlights queer identity terms across the web using their respective pride flag gradients. The Obsidian version brings the same functionality to your notes and vault.

## Features

- Automatically highlights queer identity terms with their pride flag colours
- Supports 50+ queer identities and orientations
- Uses linear gradients for multi-colour flags
- Case-insensitive matching
- Whole-word matching to avoid false positives
- Ignores code blocks, inline code, and other non-text elements
- Highlighting only shows in reading mode to avoid recursive rendering

## Installation

1. Download the latest release from the [GitHub repository](https://github.com/Yeosangist/obsidian-queer-text)
2. Extract the plugin folder to your Obsidian vault's `.obsidian/plugins/` directory
3. Enable the plugin in Obsidian's Community Plugins settings

## Supported Identities

The plugin includes flag colours for a wide range of queer identities, including:

- Rainbow / LGBTQ+ / Pride
- Gay men (achillean, mlm)
- Lesbian (wlw)
- Bisexual
- Pansexual
- Transgender
- Non-binary (enby)
- Asexual
- Aromantic
- AroAce
- Demisexual / Demiromantic
- Genderfluid / Genderqueer
- Agender
- Bigender
- Pangender
- Omnisexual
- Polysexual
- Intersex
- Two-spirit
- Sapphic
- Questioning
- Polyamorous
- Abrosexual
- Graysexual / Grayromantic
- Demigender / Demiboy / Demigirl
- Genderflux
- Genderfae / Genderfaun
- Xenogender
- Lithromantic / Akoiromantic
- Fraysexual
- Cupiosexual / Cupioromantic
- Aegosexual
- Trigender
- Multigender
- Polygender
- Androgyne
- Neutrois
- Maverique
- Omnigender
- Aporagender
- Gendervoid
- Greygender
- Quoiromantic

## Customization

You can add, remove, or modify flag entries by editing the `FLAGS` array in `main.js`. Each entry has:

- `words`: An array of words to match (e.g., `['queer', 'lgbtq']`)
- `colors`: An array of hex colour codes for the flag, from left to right

Example:
```javascript
{
    words: ['queer', 'lgbtq'],
    colors: ['#E40303', '#FF8C00', '#FFED00', '#008026', '#004DFF', '#750787']
}
```

## Configuration Options

The plugin's behaviour can be configured by modifying constants in `main.js`:

- `CASE_INSENSITIVE`: Enable case-insensitive matching (default: `true`)
- `WHOLE_WORDS_ONLY`: Match whole words only, not substrings (default: `true`)
- `IGNORED_ELEMENTS`: HTML elements to skip (code blocks, inputs, etc.)

## Compatibility

- Obsidian Desktop
- Obsidian Mobile
- All themes (uses CSS variables for compatibility)

## Credits

- **Author**: Yeosangist
- **Original Userscript**: [Queer Flag Highlighter](https://github.com/Yeosangist/queer-flag-text)

## License

This plugin is released under the GPLv3 License.

## Issues & Contributions

If you encounter issues or would like to contribute additional flags, please visit the [GitHub repository](https://github.com/Yeosangist/obsidian-queer-text).
