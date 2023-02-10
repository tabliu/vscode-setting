# vscode-setting

> 整理关于 `vs code` 编辑器常用的自定义配置

```json
{
  // vscode默认启用了根据文件类型自动设置tabsize的选项
  "editor.detectIndentation": false,
  "editor.tabSize": 2,
  "editor.fontSize": 14,
  "editor.lineHeight": 24,
  "editor.renderLineHighlight": "none",
  "editor.renderWhitespace": "trailing",
  "editor.fontFamily": "Cascadia Code, Fira Code, Source Code Pro, JetBrains Mono, Meslo LG S DZ for Powerline, Menlo, Monaco, 'Courier New', monospace",
  "editor.cursorBlinking": "smooth",
  "editor.multiCursorModifier": "ctrlCmd",
  //保存自动格式化
  "editor.formatOnSave": false,
  "editor.formatOnPaste": false,
  "editor.fontLigatures": true,
  "editor.hover.delay": 5000,
  // 是否允许自定义的snippet片段提示,比如自定义的vue片段开启后就可以智能提示
  "editor.snippetSuggestions": "top",
  "editor.wordWrap": "on",
  "editor.wordSeparators": "./\\()\"':,.;<>~!@#$%^&*|+=[]{}`~?",
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true,
    "source.organizeImports": false
  },
  "editor.renderControlCharacters": true,
  "editor.quickSuggestions": {
    "strings": true
  },
  "editor.foldingMaximumRegions": 10000,
  "editor.unicodeHighlight.invisibleCharacters": false,
  "editor.unicodeHighlight.ambiguousCharacters": false,
  "editor.language.brackets": [],
  "merge-conflict.autoNavigateNextConflict.enabled": true,
  "workbench.startupEditor": "newUntitledFile",
  "workbench.iconTheme": "vscode-great-icons",
  "files.autoSave": "afterDelay",
  "minapp-vscode.disableAutoConfig": true,
  //  #让函数(名)和后面的括号之间加个空格
  "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
  "cSpell.userWords": [
    "Alipay",
    "aolin",
    "appinfo",
    "blackvip",
    "checklogin",
    "cnpm",
    "createtime",
    "datetime",
    "devtool",
    "echarts",
    "ehome",
    "esbuild",
    "FONTON",
    "foton",
    "ftej",
    "kuanghua",
    "Lazyload",
    "linebreak",
    "linkhomepage",
    "loginname",
    "managementbly",
    "mkcert",
    "mockjs",
    "musnow",
    "noredirect",
    "nprogress",
    "ollin",
    "opreation",
    "overrided",
    "payingmember",
    "pinia",
    "prefetch",
    "promotepage",
    "pxtorem",
    "rocar",
    "svgicon",
    "tabliu",
    "tinymce",
    "tradingvolume",
    "uglifyjs",
    "unocss",
    "unplugin",
    "updatetime",
    "uploader",
    "Vant",
    "Vconsole",
    "Vetur",
    "vsvg",
    "vueuse",
    "vuex",
    "webpack's",
    "wechat",
    "wxss",
    "ZNRRMHD"
  ],
  "diffEditor.ignoreTrimWhitespace": false,
  //配置 ESLint 检查的文件类型
  "eslint.validate": ["javascript", "javascriptreact", "html", "vue"],
  //保存时eslint自动修复错误
  "eslint.autoFixOnSave": false,
  "eslint.alwaysShowStatus": true,
  "markdown.extension.toc.plaintext": true,
  "markdown.extension.toc.orderedList": true,
  "workbench.colorCustomizations": {
    "editorIndentGuide.activeBackground": "#00ff00"
  },
  "vsicons.projectDetection.autoReload": true,
  "explorer.confirmDelete": false,
  "extensions.ignoreRecommendations": true,
  "git-graph.commitDetailsView.autoCenter": false,
  "git-graph.commitDetailsView.fileView.fileTree.compactFolders": false,
  "bracketPairColorizer.activeScopeCSS": [
    "borderStyle : solid",
    "borderWidth : 1px",
    "borderColor : {color}; opacity: 0.5"
  ],
  "better-comments.tags": [
    {
      "tag": "!",
      "color": "#FF2D00",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "?",
      "color": "#3498DB",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "//",
      "color": "#404040",
      "strikethrough": true,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "todo",
      "color": "#FF8C00",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "*",
      "color": "#98C379",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    }
  ],
  "window.zoomLevel": 2,
  "todo-tree.general.tags": ["BUG", "HACK", "FIXME", "TODO", "XXX", "[ ]", "[x]"],
  "todo-tree.regex.regex": "(//|#|<!--|;|/\\*|^|^\\s*(-|\\d+.))\\s*($TAGS)",
  "terminal.integrated.tabs.enabled": true,
  "security.workspace.trust.untrustedFiles": "open",
  "vsicons.dontShowNewVersionMessage": true,
  "terminal.integrated.gpuAcceleration": "off",
  "security.workspace.trust.enabled": false,
  "faker.locale": "zh_CN",
  "filesize.displayInfoOnTheRightSideOfStatusBar": true,
  "git.alwaysSignOff": true,
  "git.suggestSmartCommit": false,
  "files.trimTrailingWhitespace": true,
  //根据文件后缀名定义vue文件类型
  "files.associations": {
    "*.vue": "vue"
  },
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[css]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[vue]": {
    "editor.defaultFormatter": "Vue.volar"
  },
  // prettier的配置 start
  // 让prettier使用eslint的代码格式进行校验
  "prettier.eslintIntegration": true,
  "prettier.printWidth": 120, // 超过最大值换行
  "prettier.tabWidth": 2, // 缩进字节数
  "prettier.useTabs": false, // 缩进不使用tab，使用空格
  "prettier.semi": true, // 句尾添加分号
  // 使用单引号代替双引号,false 不替换
  "prettier.singleQuote": true,
  // 默认值。因为使用了一些折行敏感型的渲染器（如GitHub comment）而按照markdown文本样式进行折行
  "prettier.proseWrap": "preserve",
  //  (x) => {} 箭头函数参数只有一个时是否要有小括号。avoid：省略括号
  "prettier.arrowParens": "avoid",
  // 在对象，数组括号与文字之间加空格 "{ foo: bar }"
  "prettier.bracketSpacing": true,
  // 结尾是 \n \r \n\r auto，参数类型：lf / crlf / cr / auto，默认值：lf
  "prettier.endOfLine": "lf",
  "prettier.htmlWhitespaceSensitivity": "ignore",
  // 不使用prettier格式化的文件填写在项目的.prettierignore文件中
  "prettier.ignorePath": ".prettierignore",
  // 在jsx中把'>' 是否单独放一行
  "prettier.jsxBracketSameLine": false,
  // 在jsx中使用单引号代替双引号
  "prettier.jsxSingleQuote": false,
  // 格式化的解析器，默认是babylon
  "prettier.parser": "babylon",
  // Require a 'prettierconfig' to format prettier
  "prettier.requireConfig": false,
  //不让prettier使用stylelint的代码格式进行校验
  "prettier.stylelintIntegration": false,
  // 在对象或数组最后一个元素后面是否加逗号: es5 / none / all，默认值：es5
  "prettier.trailingComma": "none",
  // 不让prettier使用tslint的代码格式进行校验
  "prettier.tslintIntegration": false,
  // 每行单个属性
  "prettier.singleAttributePerLine": true,
  // prettier的配置 end
  "liveServer.settings.donotShowInfoMsg": true,
  "tabnine.experimentalAutoImports": true,
  "workbench.colorTheme": "SynthWave '84",
  "workbench.sideBar.location": "right",
  "workbench.editor.enablePreview": false
}
```
