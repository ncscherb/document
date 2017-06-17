[TOC]
# markdown编辑平台搭建
## vim编辑markdown
### 1. 安装
- vim markdown 安装网址:http://www.jianshu.com/p/24aefcd4ca93
- node.js 安装网址：http://jingyan.baidu.com/article/dca1fa6f48f478f1a5405272.html
### 2. vim-markdown插件设置及快捷键
- url:https://github.com/plasticboy/vim-markdown
- 设置内容：
	- disable_folding
	- change fold style
	- set header fold level
- 快捷键
	- [[、]]、][
- command
The following 
	- requires :filetype plugin on.
    1. `:HeaderDecrease`:
    Decrease level of all headers in buffer: h2 to h1, h3 to h2, etc.
    If range is given, only operate in the range.
    If an h1 would be decreased, abort.
    For simplicity of implementation, Setex headers are converted to Atx.
    2. `:HeaderIncrease`: Analogous to :HeaderDecrease, but increase levels instead.
    3. `:SetexToAtx`:
    Convert all Setex style headers in buffer to Atx.
    If a range is given, e.g. hit : from visual mode, only operate on the range.
    4. `:TableFormat`: Format the table under the cursor like this.
    Requires Tabular.
    The input table must already have a separator line as the second line of the table. That line only needs to contain the correct pipes |, nothing else is required.
    5. `:Toc`: create a quickfix vertical window navigable table of contents with the headers.
    Hit <Enter> on a line to jump to the corresponding line of the markdown file.
    6. `:Toch`: Same as :Toc but in an horizontal window.
    7. `:Toct`: Same as :Toc but in a new tab.
    8. `:Tocv`: Same as :Toc for symmetry with :Toch and :Tocv.


