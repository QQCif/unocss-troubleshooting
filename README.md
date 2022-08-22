
## The issue

VSCode stuck at Initializing JS/TS language features. After running extension bisect, seems caused by unocss extension. VSCode works fine if I disable unocss extension. The folder opened in VSCode is a vite react typescript project without unocss installed. There's also a file named __unconfig_vite.config.ts generated under project root. [Link to original issue page](https://github.com/unocss/unocss/issues/1432)

## How to reproduce the issue

1. Clone this repo
2. Use `yarn` to install dependencies
3. Open project in vscode
4. Make sure unocss extension is enabled
5. __unconfig_vite.config.ts is generated
6. Open any ts/tsx file. "Initializing JS/TS language features" shows up in status bar and never goes away.