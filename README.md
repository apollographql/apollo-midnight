# Apollo Midnight Visual Studio Code theme

![Screenshot of the Apollo Midnight VS Code theme](https://raw.githubusercontent.com/jglovier/apollo-midnight/master/screenshot.png)

The Apollo Midnight VC Code color theme is based on the color palette of Apollo Studio's GraphQL Explorer in dark mode.

:warning: :construction: THIS THEME IS STILL IN DEVELOPMENT :warning: :construction:

## Install

From Marketplace:

1. Go to the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=jglovier.apollo-midnight-color-theme)
2. Click "Install"

From VS Code:

1. Go to **Extensions** in the VS Code Activity Bar (`View -> Extensions`)
2. Search for `apollo midnight color theme` by **Joel Glovier**
3. Click **Install** to install it
4. Set the theme as your active color theme (`Cmd + Shift + P -> Preferences: Color Theme -> Apollo Midnight`)

## Development (internal)

Some helpful docs for working on this theme:
- [Color Theme](https://code.visualstudio.com/api/extension-guides/color-theme) - general context on working with Color Themes in VS Code, including making user customizations to a given them, and publishing your own themes.
- [Theme Color](https://code.visualstudio.com/api/references/theme-color) - contains all of the different customizable elements of VS Code, and what their identifiers are.
- [Publishing Extensions](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) - how to guide on getting your theme published into the VS Code marketplace.
- [Extension Manifest](https://code.visualstudio.com/api/references/extension-manifest) - definitions for what can go in your theme manifest, used for publishing in the VS Code marketplace.
- [TestMate syntax Scope Naming](https://www.sublimetext.com/docs/3/scope_naming.html) - a guide to the syntax structure used in VS Code syntax theming (you may not need to refer to this if you just use VS Code's built in [Scope Inspector](https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide#scope-inspector) to identify syntax scope on a case by case basis).
- [Creating a VS Code Theme](https://css-tricks.com/creating-a-vs-code-theme/) by [Sarah Drasner](https://github.com/sdras) - a helpful walk through of what it's like to create a VS Code Theme and a recommended order to do stuff in.

**Note:** if you want to preview your customizations immediately on your existing editor windows (instead of using VS Code's "run theme" workflow using F5), you can make your changes in your `settings.json` file where they will be applied globally immediately. Then you can copy and paste those into your actual theme file.