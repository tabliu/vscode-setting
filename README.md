# vscode-setting

> 整理关于 `vs code` 编辑器常用的自定义配置

```json
{
  // VScode 主题配置
  "editor.tabSize": 2,
  "editor.wordWrapColumn": 100,
  "editor.fontSize": 18,
  "editor.fontFamily": "YaHei Consolas Hybrid, Consolas, Courier New, monospace",
  "editor.find.autoFindInSelection": false,
  "editor.showFoldingControls": "always",
  "editor.autoIndent": false,
  "editor.scrollBeyondLastLine": false,
  "editor.tabCompletion": "off",
  "editor.lineHeight": 24,
  "editor.cursorBlinking": "smooth",
  "editor.renderLineHighlight": "none",
  "editor.renderWhitespace": "none",
  "editor.wordSeparators": "./\\()\"':,.;<>~!@#$%^&*|+=[]{}`~?",
  "editor.wordWrap": "on",
  "editor.formatOnPaste": false,
  "editor.multiCursorModifier": "ctrlCmd",
  "editor.snippetSuggestions": "top",
  "editor.renderControlCharacters": true,
  // 保存时设置文件的格式。格式化程序必须可用，不能自动保存文件，并且不能关闭编辑器。
  "editor.formatOnSave": true,
  // VScode文件配置
  // 排除文件搜索区域，比如node_modules(贴心的默认设置已经屏蔽了)
  "files.exclude": {
    "**/.idea": true,
    "**/yarn.lock": true,
    "**/tmp": true,
    "**/.git": false
  },
  "files.trimTrailingWhitespace": true,
  // 配置文件关联，以便启用对应的智能提示，比如wxss使用css
  "files.associations": {
    "*.vue": "vue",
    "*.wxss": "css",
    "*.cjson": "jsonc",
    "*.wxs": "javascript",
    "*.wxml": "html"
  },
  // 文件末尾增加空行
  "files.insertFinalNewline": true,
  "files.autoSave": "afterDelay",
  "files.eol": "\n",
  "workbench.iconTheme": "material-icon-theme",
  "workbench.colorTheme": "Material Theme Ocean High Contrast",
  "workbench.startupEditor": "newUntitledFile",
  "workbench.sideBar.location": "left",
  // 控制台显示系统控制台
  //"terminal.integrated.shell.windows": "C:\\Windows\\System32\\cmd.exe",
  // 开启 vscode 文件路径导航
  "breadcrumbs.enabled": true,
  // 格式化快捷键 shirt+alt+F
  // 是否开启eslint检测
  "eslint.enable": true,
  // 设置 eslint 保存时自动修复
  "eslint.autoFixOnSave": true,
  // eslint 检测文件类型
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "vue-html",
    {
      "language": "html",
      "autoFix": true
    },
    {
      "language": "vue",
      "autoFix": true
    }
  ],
  "eslint.run": "onSave",
  // vetur 的自定义设置
  "vetur.format.defaultFormatterOptions": {
    // 对属性进行换行。
    // - auto: 仅在超出行长度时才对属性进行换行。
    // - force: 对除第一个属性外的其他每个属性进行换行。
    // - force-aligned: 对除第一个属性外的其他每个属性进行换行，并保持对齐。
    // - force-expand-multiline: 对每个属性进行换行。
    // - aligned-multiple: 当超出折行长度时，将属性进行垂直对齐。
    "js-beautify-html": {
      "wrap_line_length": 80,
      "wrap_attributes": "force-expand-multiline",
      "end_with_newline": false
    },
    "prettier": {
      "semi": false, //不使用分号结尾
      "singleQuote": true, //使用单引号
      "eslintIntegration": true //开启 eslint 支持
    }
  },
  "vetur.validation.template": false,
  "vetur.format.defaultFormatter.html": "js-beautify-html",
  "vetur.format.defaultFormatter.ts": "vscode-typescript",
  "vetur.format.defaultFormatter.css": "prettier",
  "vetur.format.defaultFormatter.less": "prettier",
  "vetur.format.defaultFormatter.scss": "prettier",
  "vetur.format.defaultFormatter.postcss": "prettier",
  //开启 eslint 支持
  "prettier.eslintIntegration": true,
  //使用单引号
  "prettier.singleQuote": true,
  //结尾不加分号
  "prettier.semi": false,
  // VScode 文件搜索区域配置
  "search.exclude": {
    "**/dist": true,
    "**/build": true,
    "**/elehukouben": true,
    "**/.git": true,
    "**/.gitignore": true,
    "**/.svn": true,
    "**/.DS_Store": true,
    "**/.idea": true,
    "**/.vscode": false,
    "**/yarn.lock": true,
    "**/tmp": true
  },
  // 配置emmet是否启用tab展开缩写
  "emmet.triggerExpansionOnTab": true,
  // 配置emmet对文件类型的支持，比如vue后缀文件按照html文件来进行emmet扩写
  "emmet.syntaxProfiles": {
    "vue-html": "html",
    "vue": "html",
    "vxml": "html",
    "javascript": "javascriptreact",
    // xml类型文件默认都是单引号，开启对非单引号的emmet识别
    "xml": {
      "attr_quotes": "single"
    }
  },
  // 在react的jsx中添加对emmet的支持
  "emmet.includeLanguages": {
    "jsx-sublime-babel-tags": "javascriptreact",
    "vue-html": "html",
    "vue": "html",
    "wxml": "html"
  },
  // 细节,配置gitlen中git提交历史记录的信息显示情况
  "gitlens.advanced.messages": {
    "suppressShowKeyBindingsNotice": true,
    "suppressUpdateNotice": true
  },
  // git是否启用自动拉取
  "git.confirmSync": false,
  "git.autofetch": false,
  "git.ignoreLegacyWarning": true,
  // By default, create file  username
  "fileheader.Author": "author",
  "fileheader.tpl": "/** * @Author: {author}  * @Date: {createTime}  * @Last Modified by:   {lastModifiedBy}  * @Last Modified time: {updateTime}  */",
  // By default, update file  username.
  "fileheader.LastModifiedBy": "author",
  // liveServer
  "liveServer.settings.port": 8888, //设置本地服务的端口号
  "liveServer.settings.root": "/", //设置根目录，也就是打开的文件会在该目录下找
  "liveServer.settings.CustomBrowser": "chrome", //设置默认打开的浏览器
  "liveServer.settings.AdvanceCustomBrowserCmdLine": "chrome --incognito --remote-debugging-port=9222",
  "liveServer.settings.NoBrowser": false,
  "liveServer.settings.donotShowInfoMsg": true,
  "liveServer.settings.donotVerifyTags": true,
  "explorer.confirmDragAndDrop": false,
  "explorer.confirmDelete": false,
  "view-in-browser.customBrowser": "chrome",
  "minapp-vscode.disableAutoConfig": true,
  "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe",
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  }
}
```
