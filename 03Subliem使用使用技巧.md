[TOC]

##1. markdown 插件不兼容问题:
>在Sublime Text 3 MarkdownEditing插件打开md文件默认的主题很丑，而且文字居中，左侧有大片空白，需要修改配置文件调整一下。
流程:
### 1. 修改setting
>ctrl+shift+p打开命令输入，打开Preference: MarkdownEditing GFM Setting: User
ctrl+shift+p打开命令输入，打开Preference: MarkdownEditing GFM Setting: Default
将Preference: MarkdownEditing Setting: Default对应文件内容复制到Preference: MarkdownEditing Setting: User中
在Preference: MarkdownEditing Setting: User中修改

```
    "color_scheme": "Packages/MarkdownEditing/MarkdownEditor.tmTheme",
    "color_scheme": "Packages/MarkdownEditing/MarkdownEditor-Dark.tmTheme",
```
>改为

```
// "color_scheme": "Packages/MarkdownEditing/MarkdownEditor.tmTheme",
 "color_scheme": "Packages/MarkdownEditing/MarkdownEditor-Dark.tmTheme",

```
###3. 修改主题为深色，与sublime主题一一致



```
 //Layout
"draw_centered": false, // 改为false，原始值为true
"word_wrap": true,
"wrap_width": 120, // 每行字符数上限
"rulers": [],
```


配置完毕。

# Markdown语法插件： Github Markdown Snippets
>  Thanks for Github Markdown Snippets! (✿✪‿✪｡)
>  To report bugs and request features - https://github.com/praveenpuglia/github_markdown_snippets
  A consolidated guide is available at - http://praveenpuglia.github.io/github_markdown_snippets 
  Type a tag name and hit tab. That's it! ｡◕‿◕｡
  ✿ Long tags like `blockquote` are shortened for power use.
  
 > 〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜
  List of Tab Triggers
  〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜〜
```markdown
  h1              // Heading 1
  h2              // Heading 2
  h3              // Heading 3
  h4              // Heading 4
  h5              // Heading 5
  h6              // Heading 6
  b               // Bold
  i               // Italic
  bq              // Blockquote
  strike          // Strikeout
  hr              // Horizontal Rule, Divider
  code            // Inline Code
  pre             // Code Block with language based highlighting.
  a               // Anchor
  img             // Image
  ol              // Ordered List
  ul              // Unordered List
  table           // Table
```
