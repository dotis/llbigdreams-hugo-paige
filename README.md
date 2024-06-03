Edit website content in the `/content/` directory. 
Markdown or html can be used.
A github action to build & deploy to github pages is in `.github/workflows`, so any changes made here should show up there within a few minutes (cache clearing sometimes needed).

The nav menu is configured in `/hugo.toml`.

The "look" of the site is largely inherited from the Paige theme but is customized by the `/layouts/partials/paige/style-last.css` file.

Run a local dev server:
```bash
hugo serve -D --disableFastRender --logLevel debug --ignoreCache --printPathWarnings --printUnusedTemplates
```

This site is based on the (MIT-licensed) [Paige Theme](https://themes.gohugo.io/themes/paige/).
Rather than being set up as a module, all content for the theme is duplicated here under `/themes/page/`. 
This means that the theme files can be edited here but also that the theme will not be updated automatically.
