# Neon Genesis Evangelion 2 Chinese Localization

A [Slidev](https://sli.dev/) presentation about the Chinese localization of
*Neon Genesis Evangelion 2: The Created World*. It covers encoding, fonts, text
reconstruction, and runtime patches for PSP games.

## Presentation Outline

1. **PSP Fan Translation Background**
   - The scale and history of Chinese PSP fan translations
   - The different challenges in English and Chinese fan translations
   - Missing Chinese glyphs in Shift JIS
   - The standard method: reuse Shift JIS byte ranges and replace glyphs
2. **The Game and Its Reverse Engineering**
   - An overview of the PSP version of *Neon Genesis Evangelion 2*
   - The community's work on the game resources, text, and fonts
3. **Encoding and Fonts**
   - The data path from Shift JIS to the UCS-2 format used by `sceFont`
   - Hooks for the `sceFont` character APIs
   - A custom Shift JIS to UTF-16 mapping
4. **The Memory Text System**
   - The game's fixed-slot sentence templates
   - Word-order problems during translation from Japanese to Chinese
   - Runtime text reconstruction after moving the object into the template
5. **Patch Architecture**
   - The roles of the Loader, original game, and Runtime Plugin
   - Module loading, address relocation, and patch installation
   - Runtime changes before the game starts
6. **Demo and Acknowledgments**
   - The current localization and project status
   - Other Evangelion localization projects for the PSP
   - Contributors and related open-source projects

## Local Development

```bash
yarn install
yarn dev
```

The development server runs at <http://localhost:3030> by default.

```bash
yarn build   # Build the static site in dist/
yarn export  # Export the presentation
```

## Project Structure

- [`slides.md`](./slides.md): presentation content
- [`public/`](./public/): image and video assets
- [`components/`](./components/): Slidev and Vue components
- [`.github/workflows/deploy-pages.yml`](./.github/workflows/deploy-pages.yml): GitHub Pages deployment workflow
