# sublime-text-usage
总结一些sublime text 的使用技巧，收集常用插件，提高coding效率

本笔记所有内容大部分来自网络，以及自己的一些使用经验。网络内容我会注明出处，如果有侵权问题请联系我删除。
Most of these notes are quoted from internet, and some experience of mine. If any infringement, please contact me at the deleted.

#Tools
###From [WASIL.ORG](http://wasil.org/sublime-text-3-perfect-php-development-set-up)
1. **Package Control** (https://sublime.wbond.net)
Thanks to this little piece of software all other plugins are easily installed.
2. **SublimeCodeIntel** (https://github.com/SublimeCodeIntel/SublimeCodeIntel)
This is package I use all the time. Its job is to provide hints related to function, object, variable etc. names. It also hints what methods and parameters are available in objects/classes. It’s based on Komodo CodeIntel and sometimes it has some problems working at all. But most of the time it rocks :)
3. **SublimeLinter** (https://sublime.wbond.net/packages/SublimeLinter)
This package does full-time job for me – it constantly watches what I write and instantly lets me know if something is not OK, for example I forget semi-colon or brackets.

  > **(update)**

  > From version 3 and up, SublimeLInter has become modular. This means, that you have to install main package first, and then plugin/module for every language you need support for. Each plugin has it’s own set of requirements, so please make sure you read them thoroughly.
  For PHP + JavaScript development I’m using:

  > - [SublimeLinter-php](https://sublime.wbond.net/packages/SublimeLinter-php)
  > - [SublimeLinter-jshint](https://packagecontrol.io/packages/SublimeLinter-jshint)
  > - [SublimeLinter-json](https://sublime.wbond.net/packages/SublimeLinter-json)
  > - and [SublimeLinter-csslint](https://sublime.wbond.net/packages/SublimeLinter-csslint)

4. **SideBarEnhancements** (https://sublime.wbond.net/packages/SideBarEnhancements)
Provides great new options when right-clicking on sidebar elements (files/folders). Very convenient.
5. **VCS Gutter** (https://sublime.wbond.net/packages/VCS%20Gutter)
Lately I don’t imagine working without this one. Every day I use Git and Mercurial and this plugins gives me real-time information about what was changed (or added/removed) in current file using symbols in left-hand edit window gutter.
6. **SFTP**, paid (http://wbond.net/sublime_packages/sftp)
Great package enabling very comfortable use of SFTP, FTP and FTPS. It supports remote folders browsing, editing and synchronization between local and remote files. Also regular upload, download, save or file open.
7. **Tortoise** (on Windows only) (http://wbond.net/sublime_packages/tortoise)
I use it as a complementary package to SideBarGit if I’m working in Windows environment. It doesn’t have so many features but those what it provide are very helpfull and intuitive.If you like Tortoise Git but you are working on Linux you might want to check out RabbitVCS. It isn’t integrated with ST2, but it provides comfortable right-mouse-click Git GUI.
8. **sublime-github** (https://github.com/bgreenlee/sublime-github)
Every developer should use code snippets of some kind. I use Gist provided by GitHub and this package enables me to use them instantly (save/paste).
9. **Tag** (https://github.com/SublimeText/Tag)
It is fine plugin, but now ST3 supports tag matching, so I don’t need it any more.
10. **PhpDoc** (https://sublime.wbond.net/packages/PhpDoc)
Great plugin aiding writing documentation docblocks for PHPDocumentor.
11. **Phpcs** (http://soulbroken.co.uk/code/sublimephpcs)
This package adds support for PHP_CodeSniffer to ST2. It checks if you code is written according to one of the standards. Just pick one: Zend, PEAR.. and more :) Check out PHP_CodeSniffer website for configuration details.
12. **TrailingSpaces** (https://github.com/SublimeText/TrailingSpaces)
Small horror of every code – empty spaces at lines ends, at the end of file. Especially troublesome if you are working on the code with other developers, who might use different editors/IDEs which might interpret them (empty spaces) differently.
13. **BracketHighlighter** (https://github.com/facelessuser/BracketHighlighter)
Same situation as with Tag plugin. In my everyday coding ST3 bracket highlighting capabilities of ST3 are good enough. It is still great plugin though.
14. **Sublime Function Name Display** (https://github.com/akrabat/SublimeFunctionNameDisplay)
Displays in bottom bar name of a function (or method) in which our cursor is placed. Simple and helpful.
15. **Terminal** (http://wbond.net/sublime_packages/terminal)
Using Git or maybe some PEAR packages you might need to switch to console from time to time and do some magic. Maybe use Zend Tool or “bake” something ;) It’s just what this plugin is for.
16. **Xdebug Client** (https://sublime.wbond.net/packages/Xdebug%20Client)
Lately my favorite Xdebug client for ST3. Works great and allows to use all of Xdebug debugging capabilities.

If you know any plugin worth mentioning, then let me know – I’ll be glad to add it to my list. Any suggestions? :)

##Hot key
Default Keymap [@jikeytang](https://github.com/jikeytang/sublime-text)

1. Ctrl+L             选择整行（按住-继续选择下行） 
2. Ctrl+Shift+K(shhift+del)     删除整行，  ctrl + KK 从光标处删之行尾，Ctrl+K Backspace 从光标处删除至行首
3. Ctrl+Shift+D       复制光标所在整行，插入在该行之前  
4. Ctrl+D             选词 （按住-继续选择下个相同的字符串，再按，可跳到相应的方法定义处
5. Ctrl+Shift+M       选择括号内的内容（按住-继续选择父括号） 
6. Ctrl+/             注释整行（如已选择内容，同“Ctrl+Shift+/”效果）
7. Ctrl + alt + /     取消注释 
8. Ctrl+Shift+UP      与上行互换  ctrl + shift + up: 列模式编辑  
9. Ctrl + R           跳转当前页的目标方法
10. Ctrl+K + U        大写
11. Ctrl+K + L        小写
12. 鼠标中间           列模式编辑
13. Ctrl+Shift+[]     代码折叠
14. ctrl+k ctrl+1:    折叠所有代码 
15. Ctrl + K,B        打开侧边栏
16. ctrl + 回车：　　   光标后插入行，　Ctrl+Shift+Enter 光标前插入行
17. ctrl + m:         匹配括号
18. vim mode下        查找上一个下一个的快捷键是 是* #
19. ctrl +z, y:       撤销，恢复撤销
20. alt + .:          闭合当前标签
21. Ctrl+F2:          设置书签
22. F2:               下一个书签
23. Shift+F2:         上一个书签
24. ctrl + p:         即时的文件切换
25. ctrl + shift + a: 选择标签内的内容 
26. ctrl + 单击：      多行随意位置添加光标
27. alt + F3( mac: ctrl + command + g): 选择页面中所有相同的词
28. ctrl + F3:        跳转到下一个选中的词    
29. Ctrl+Shift+P Set Syntax:html : 设置文件类型
30. Shift + 右键:     连续多行光标选中 (by Gary Gauh)
