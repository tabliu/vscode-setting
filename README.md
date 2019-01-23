# vscode-config

> 整理关于vscode编辑器常用的自定义配置

```json
{
    // VScode主题配置
    "editor.fontSize": 18,
    "editor.fontFamily": "YaHei Consolas Hybrid, Consolas, 'Courier New', monospace",
    "editor.find.autoFindInSelection": true,
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

    // 控制台显示系统控制台
    "terminal.integrated.shell.windows": "C:\\Windows\\System32\\cmd.exe",

    // 文件末尾增加空行
    "files.insertFinalNewline": true,

    // tab 大小为2个空格
    "editor.tabSize": 2,

    // 100 列后换行
    "editor.wordWrapColumn": 100,

    // 开启 vscode 文件路径导航
    "breadcrumbs.enabled": true,

    // prettier 设置语句末尾不加分号
    "prettier.semi": false,

    // prettier 设置强制单引号
    "prettier.singleQuote": true,

    // 选择 vue 文件中 template 的格式化工具
    "vetur.format.defaultFormatter.html": "prettyhtml",

    // 显示 markdown 中英文切换时产生的特殊字符
    "editor.renderControlCharacters": true,

    // 设置 eslint 保存时自动修复
    "eslint.autoFixOnSave": true,

    // eslint 检测文件类型
    "eslint.validate": [
        "javascript",
        "javascriptreact",
        {
        "language": "html",
        "autoFix": true
        },
        {
        "language": "vue",
        "autoFix": true
        }
    ],

    // vetur 的自定义设置
    "vetur.format.defaultFormatterOptions": {
        "prettier": {
        "singleQuote": true,
        "semi": false
        },
        "wrap_attributes": "force-aligned"
    },

    // 格式化快捷键 shirt+alt+F
    // prettier进行格式化时是否安装eslint配置去执行，建议false
    "prettier.eslintIntegration": true,
    "vetur.validation.template": false,
    "vetur.format.defaultFormatter.ts": "vscode-typescript",

    // 是否允许自定义的snippet片段提示,比如自定义的vue片段开启后就可以智能提示
    "editor.snippetSuggestions": "top",
    "workbench.iconTheme": "material-icon-theme",
    "workbench.colorTheme": "Atom One Dark",
    "workbench.startupEditor": "newUntitledFile",
    "files.trimTrailingWhitespace": true,

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

    // 排除文件搜索区域，比如node_modules(贴心的默认设置已经屏蔽了)
    "files.exclude": {
        "**/.idea": true,
        "**/yarn.lock": true,
        "**/tmp": true
    },

    // 配置文件关联，以便启用对应的智能提示，比如wxss使用css
    "files.associations": {
        "*.vue": "vue",
        "*.wxss": "css"
    },

    // 配置emmet是否启用tab展开缩写
    "emmet.triggerExpansionOnTab": true,

    // 配置emmet对文件类型的支持，比如vue后缀文件按照html文件来进行emmet扩写
    "emmet.syntaxProfiles": {
        "vue-html": "html",
        "vue": "html",
        "javascript": "javascriptreact",
        // xml类型文件默认都是单引号，开启对非单引号的emmet识别
        "xml": {
            "attr_quotes": "single"
        }
    },

    // 在react的jsx中添加对emmet的支持
    "emmet.includeLanguages": {
        "jsx-sublime-babel-tags": "javascriptreact"
    },

    // 细节,配置gitlen中git提交历史记录的信息显示情况
    "gitlens.advanced.messages": {
        "suppressShowKeyBindingsNotice": true,
        "suppressUpdateNotice": true
    },

    // git是否启用自动拉取
    "git.confirmSync": false,
    "git.autofetch": true,
    "git.ignoreLegacyWarning": true,

    // 保存时设置文件的格式。格式化程序必须可用，不能自动保存文件，并且不能关闭编辑器。
    "editor.formatOnSave": false,

    // 启用/禁用默认 HTML 格式化程序
    "html.format.enable": false,

    // By default, create file  username
    "fileheader.Author": "liuyun",

    // By default, update file  username.
    "fileheader.LastModifiedBy": "liuyun",
    "vsicons.dontShowNewVersionMessage": true,
    "liveServer.settings.donotShowInfoMsg": true,

    // liveServer
    "liveServer.settings.port": 8888, //设置本地服务的端口号
    "liveServer.settings.root": "/", //设置根目录，也就是打开的文件会在该目录下找
    "liveServer.settings.CustomBrowser": "chrome", //设置默认打开的浏览器
    "liveServer.settings.AdvanceCustomBrowserCmdLine": "chrome --incognito --remote-debugging-port=9222",
    "liveServer.settings.NoBrowser": false,
    "explorer.confirmDragAndDrop": false,
    "liveServer.settings.donotVerifyTags": true,
    "vetur.format.defaultFormatter.js": "vscode-typescript",
    "view-in-browser.customBrowser": "chrome",
    "scss.lint.idSelector": "warning",
}
```
