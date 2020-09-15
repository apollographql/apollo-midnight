# Apollo Midnight Visual Studio Code theme

![Screenshot of the Apollo Midnight VS Code theme](https://raw.githubusercontent.com/apollographql/apollo-midnight/master/screenshot.png)

The Apollo Midnight VC Code color theme is based on the color palette of Apollo Studio's GraphQL Explorer in dark mode.

## Install

From Marketplace:

1. Go to the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=apollographql.apollo-midnight-color-theme)
2. Click "Install"

From VS Code:

1. Go to **Extensions** in the VS Code Activity Bar (`View -> Extensions`)
2. Search for `apollo midnight color theme`
3. Click **Install** to install it
4. Set the theme as your active color theme (`Cmd + Shift + P -> Preferences: Color Theme -> Apollo Midnight`)

## Customizing

Do you like this theme, but want to customize it a bit? You can easily do that by adding custom rules to your VS Code user settings file that overide theme defaults. Here's how:

```
{
  "workbench.colorCustomizations": {
      "[Apollo Midnight]": {
        "activityBar.background": "#000000",
        "activityBar.border": "#ff0000",
        "sideBar.background": "#000000",
        "sideBar.border": "#ff0000",
        "sideBar.foreground": "#ffffff"
      }
  }
}
```

[Read more](https://code.visualstudio.com/api/extension-guides/color-theme#workbench-colors) about customizing themes in your user `settings.json` file.

You may also want to refer to the [Theme Color docs](https://code.visualstudio.com/api/references/theme-color#panel-colors) that tell you what keys to use to select parts of the VS Code UI. 

If you wish to customize syntax, you need to do that with `editor.tokenColorCustomizations`, which you'll put under the `workbench.colorCustomizations` declarations. [More about that here](https://code.visualstudio.com/api/extension-guides/color-theme#syntax-colors).

## Contributing

**I found something that isn't styled.** Thanks for noticing! Feel free to [open an issue](https://github.com/apollographql/apollo-midnight/issues) to report it and I'll ship an update as soon as I'm able. Or, feel free to propose a styling for it by submitting a [pull request](https://github.com/apollographql/apollo-midnight/pulls)! :tada:

**I don't like something the way that it is styled.** I understand, color choices can be very personal. If you think it's problematic for accessibilty, please let me know by [opening an issue](https://github.com/apollographql/apollo-midnight/issues) and I will address it as soon as I'm able (or open a pull request to propose a fix). If it is not accessibility related but you have general feedback, I still want to hear it. [Please open an issue](https://github.com/apollographql/apollo-midnight/issues). Otherwise, if it's just a matter of personal taste, feel free to overide the styles with your own custom user settings on your machine. [Here's how](https://code.visualstudio.com/api/extension-guides/color-theme#workbench-colors).

**I have an idea for something really cool.** Awesome! Great ideas are fun. :brain::zap::grinning: If your idea is something you think that everyone else would like too, open an issue to discuss it or just open a PR to propose it. If you're not sure, feel free to propose it anyway. If you just want to try out your idea for yourself, feel free to override the theme styles with your own custom user settings on your machine. [Here's how](https://code.visualstudio.com/api/extension-guides/color-theme#workbench-colors).

## Development (internal)

**Maintainer:** [@jglovier](https://github.com/jglovier/)

Some helpful docs for working on this theme:
- [Color Theme](https://code.visualstudio.com/api/extension-guides/color-theme) - general context on working with Color Themes in VS Code, including making user customizations to a given them, and publishing your own themes.
- [Theme Color](https://code.visualstudio.com/api/references/theme-color) - contains all of the different customizable elements of VS Code, and what their identifiers are.
- [Publishing Extensions](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) - how to guide on getting your theme published into the VS Code marketplace.
- [Extension Manifest](https://code.visualstudio.com/api/references/extension-manifest) - definitions for what can go in your theme manifest, used for publishing in the VS Code marketplace.
- [TestMate syntax Scope Naming](https://www.sublimetext.com/docs/3/scope_naming.html) - a guide to the syntax structure used in VS Code syntax theming (you may not need to refer to this if you just use VS Code's built in [Scope Inspector](https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide#scope-inspector) to identify syntax scope on a case by case basis).
- [Creating a VS Code Theme](https://css-tricks.com/creating-a-vs-code-theme/) by [Sarah Drasner](https://github.com/sdras) - a helpful walk through of what it's like to create a VS Code Theme and a recommended order to do stuff in.

**Note:** if you want to preview your customizations immediately on your existing editor windows (instead of using VS Code's "run theme" workflow using F5), you can make your changes in your `settings.json` file where they will be applied globally immediately. Then you can copy and paste those into your actual theme file.

**Publishing**
> Note: Publishing a new version of this theme is only meant for maintainers.

**Prerequisite**: Please follow this [guide](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) to install and login to `vsce`. Ask an existing maintainer how to get the "Personal Access Token".

1. Update [CHANGELOG.md](https://github.com/apollographql/apollo-midnight/blob/master/CHANGELOG.md), and commit latest changes to the repo.
3. Run `vsce publish [version]`. Follow the [SemVer](https://semver.org) convention and replace `[version]` with one of the following  options:
    - `patch` for bug fixes
    - `minor` for improvements
    - `major` for breaking or bigger changes
4. Push the commits and make a [new release](https://github.com/apollographql/apollo-midnight/releases/new).

## License

This project is licensed with the [MIT License](https://github.com/apollographql/apollo-midnight/blob/master/LICENSE), and created by [Joel Glovier](http://github.com/jglovier) for hack day at [Apollo](https://www.apollographql.com/careers).