# TO  Hu, Gessing and Me

给一根成年香蕉的远程共享代码修改库
-----

这是一个给你用的远程共享代码修改库。它的目的是让你能更清楚地提出代码报错、在 VS Code 里使用 Git、描述修改内容，并最终把修好的代码提交到仓库里。

## 为什么我要写这个仓库？
我希望你能更清楚地描述代码报错、修改内容和 Git 操作，这样我才能更快地帮你解决问题。

我会尽力维护整个仓库的清晰和规范，毕业后我会删掉这个仓库，或者把它改成一个公开的 Git 教程。总之，这个仓库是为了让你更好地学习，以及更清晰地描述代码问题。

## 这个仓库是怎么运行的?
你提出Issue，描述你遇到的代码问题和修改内容，我的邮箱会收到消息通知，我会尽快回复你，帮你解决问题。
或者换一种说法来说，我是一个人肉的Skill和超级节省Token 的 **能工智人**

如果有必要我会继续在这个文件中整理你遇到的问题，并给出一定的解决方法，**但是一切的前提是你能做到遇到问题的时候会提问和说明，这是你需要学习的。**

## 0. 写在前面

### 什么是Git？
Git 是一个版本控制系统，允许你跟踪代码的修改历史、协作开发、管理不同版本的代码。通过 Git，你可以在本地修改代码，然后把修改提交到远程仓库（例如 GitHub），让其他人也能看到你的改动。

### 什么是GitHub？
GitHub 是一个基于 Git 的代码托管平台，提供了一个在线界面来管理 Git 仓库。你可以在 GitHub 上创建仓库、提交代码、提 Issue、进行代码审查等。


### Git安装


参考网址：[给香蕉的Git教程](https://www.bilibili.com/video/BV1Hkr7YYEh8/)


如果你不知道什么是“代理、梯子”，或者追求速度，那么请使用以下的方法安装 Git：
参考链接：[给国内香蕉的Git安装教程](https://www.bilibili.com/video/BV1bRN2enEtV/)


按安装过程中你会使用到如下网址

> Git 官网：https://git-scm.com/
> Git第一步配置：https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup
> Gitee 官网： https://gitee.com/


课外作业
如果你对 Git 和 GitHub 还不熟悉，建议你先花点时间学习一下。可以参考以下资源：
- [Git 官方文档](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)

如果你想要在多试试Git的基本操作，你可以在以下网址学习

- [一个较为简单可视化的Git学习平台 Learn Git Branching](https://learngitbranching.js.org/)

## 快速开始/ 常见问题

```bash
报错：ModuleNotFoundError: No module named 'xxx'
原因：没有安装指定的 Python 包。

初始化conda环境
conda env list

选择你的环境
conda activate banana-env

conda init

启用另外一个终端

安装相关的包
pip install banana1
pip install banana2

```

## 你该怎么用这个仓库

### 1. 遇到代码报错时怎么提问

当你发现代码有问题，先写清楚这四项：

- 你在做什么操作？（例如：打开 `main.py`、运行 `npm start`、在 VS Code 里保存文件）
- 你期望程序做什么？（例如：希望输出一张图、希望网页能正常显示、希望保存数据）
- 你实际看到什么报错？
- 你已经试过什么方法？（例如：重新运行、复制粘贴 GPT 的代码、重启 VS Code）

示例：

> 我在 VS Code 里打开了 `src/app.js`，想运行本地项目。按 `F5` 后，终端显示 `ReferenceError: xxx is not defined`，我已经尝试把 GPT 给的代码复制粘贴进来，但报错依旧。

### 2. 报错描述要怎么写

格式建议：

1. 问题背景：你在做哪一步？
2. 现象描述：有什么错误或不对？
3. 错误信息：完整复制终端/浏览器的报错内容。最好连同出现的文件名、行号一起上传。 
4. 已尝试操作：你已经试过哪些办法？

写得好的例子：

> 背景：我正在修改 `src/index.html`，想让页面出现按钮。
> 现象：网页加载后白屏，控制台报错。
> 错误：`Uncaught TypeError: Cannot read properties of null (reading 'addEventListener') at src/main.js:45:10`
> 尝试：我把 GPT 输出的代码复制进来，重新启动了 VS Code，问题还是有。

### 2.1 报错信息该写在哪里

请把报错信息写在这个仓库的说明里，或者直接发给我，不要把错误写进代码文件里。代码文件只能放程序代码，不能放你自己的注释报错内容，否则会让程序更难运行。

最安全的方式是：

- 在这个 `README.md` 里写清楚；
- 或者在你给我的聊天/日志里直接粘贴完整报错；
- 如果你在 Git 提交说明里写，也请写在提交说明/Issue 描述里，而不是写在 `.js`、`.py`、`.html` 这些源代码里。

示例：

> 出错位置：`src/main.js`。
> 报错信息：`ReferenceError: userData is not defined at src/main.js:32:15`。
> 我已经试过：重启 VS Code、重新复制 GPT 的代码。

### 2.2 如果你要提 Issue

这个仓库最适合你提“问题描述”，也就是 GitHub Issue。Issue 是一个专门记录错误、改动建议、问题说明的地方，写在这里最清楚。

你可以按这个格式提 Issue：

- 标题（Title）：一句话说清楚问题，例如 `页面白屏 / 控制台报错`。
- 内容（Description）：把下面这些信息写清楚：
  1. 我在 `文件名` 做了什么。
  2. 期望结果是什么。
  3. 实际结果是什么。
  4. 完整报错信息。
  5. 我已经尝试过什么。
  6. 如果你改了文件，写上改动的文件名。

示例 Issue 内容：

> 标题：`页面白屏，控制台报错`
>
> 内容：
> - 我在 `src/index.html` 里加了按钮。
> - 期望结果：页面出现按钮并正常运行。
> - 实际结果：网页白屏，开发者工具控制台出现错误。
> - 错误信息：`Uncaught TypeError: Cannot read properties of null (reading 'addEventListener') at src/main.js:45:10`
> - 我已尝试：重新加载页面、复制粘贴 GPT 的代码、重启 VS Code。
> - 相关修改：我改了 `src/index.html` 和 `src/main.js`。
附上相关的截图

#### 如果你不懂怎么写：

- 先把你看到的报错原样复制粘贴在 Issue 里。
- 再写一句“我想让它做什么，我做了什么，它却报错了”。

这样我就能最快帮你定位问题。

### 2.3 常见 Python 报错该怎么描述

如果你遇到 Python 报错，可以按下面提示写给 AI 或我，不要直接在代码里改。告诉我们你看到的是哪一种错误，以及你已经做了什么。

- 导入包错误（ImportError / ModuleNotFoundError）：
  - 写法：`ImportError: No module named 'xxx'` 或 `ModuleNotFoundError: No module named 'xxx'`
  - 说明：这通常说明你没有激活正确的 Anaconda 环境，或者没有安装这个包。
  - 你可以写："我在运行 `python script.py` 时，出现 `ModuleNotFoundError: No module named 'pandas'`。我的 Anaconda 环境是 `base`，我不确定是否需要安装这个包。"

- UTF-8 支持错误：
  - 写法：`UnicodeDecodeError: 'utf-8' codec can't decode byte 0x...` 或 `SyntaxError: Non-UTF-8 code starting with '\x...'`
  - 说明：这一般和文件编码有关，说明文件不是 UTF-8 编码，或者代码里有中文字符没有正确保存。
  - 你可以写："我打开 `script.py` 运行时，提示 `UnicodeDecodeError`，我只是复制了一段中文注释进去。"

- 缩进错误（IndentationError）：
  - 写法：`IndentationError: unexpected indent` 或 `IndentationError: expected an indented block`
  - 说明：这是 Python 对缩进很严格，通常是多了空格、少了空格、混用了 Tab 和空格。
  - 你可以写："运行 `main.py` 时出现 `IndentationError: unexpected indent`，我看了一下可能是缩进不一致。"

如果你看到其它 Python 错误，也请把“完整报错信息”原样贴出来，我会帮你把这些文字解释成要改的代码。

### 3. 在 VS Code 里使用 Git 的基本操作

如果你只会复制粘贴，先记住这几个最常用步骤：

- 打开 VS Code，左侧栏点击“源代码管理”图标。
- 如果仓库已经打开，VS Code 会自动识别 Git。可以看到改动文件列表。
- 改完文件后，在“源代码管理”里写一句简单的提交说明，例如 `fix: 修复按钮事件`，然后点击提交按钮。
- 如果要同步到远程仓库，点击页面右下角的“同步更改”按钮，或者使用命令面板：`Ctrl+Shift+P` → 输入 `Git: Push`。

#### 推荐的基本 Git 习惯

- 先检查改了哪些文件。
- 不要直接在 `main` 或 `master` 上改大版本内容。
- 每次改完保存，再提交一次。
- 如果不确定，先写一句“我不懂这个改动，先提交了”，然后把问题说明给我。

### 4. 分支与合并怎么用

分支就是一个新的修改路线，避免直接改主分支。通常流程：

1. 先创建一个分支。命令很简单：
   - `git checkout -b fix-xxx` 或在 VS Code 的分支菜单里新建。
2. 在这个分支上修改代码。
3. 提交你的改动。
4. 如果你想把修改合并回主分支：
   - 切回 `main` 分支：`git checkout main`
   - 合并你的分支：`git merge fix-xxx`

如果你不熟命令，可以直接在 VS Code 里操作：

- 左下角点击当前分支名，选择“新建分支”。
- 修改完成后，在“源代码管理”里提交。
- 再切回 `main`，点击分支菜单里的“合并分支”。

> 重要：如果你只是暂时修改，建议先不要合并主分支。先把错和需求发给我，我会帮你检查。

### 5. 修改的代码怎么描述

每次你改完代码，写一句简单说明：

- 你改了什么？（例如：把 `if` 条件改成 `===`、增加了 `console.log`、修复了缺少的 `return`）
- 为什么改？（例如：因为出现报错、因为页面没有显示、因为变量未定义）
- 结果是什么？（例如：现在不报错了、页面可以正常显示了）

示例说明：

> 修改内容：修复 `src/app.js` 中 `data` 未定义的问题。
> 原因：`userData` 变量名写错，导致运行时报 `ReferenceError`。
> 结果：保存后页面不再报错，控制台正常输出。

### 6. 给你最简单的提问模板

你可以直接照着下面写：

- 我在 `文件名` 做了什么：
- 期望结果：
- 实际结果/报错：
- 相关错误信息：
- 我已尝试：
- 我改了哪几行代码（或哪个函数）：

### 7. 常用错误解决办法

>  `ModuleNotFoundError`
- 问题：`ModuleNotFoundError: No module named 'xxx'`
- 原因：没有安装指定的 Python 包。
- 解决办法：在终端中运行 `pip install xxx` 安装该包。


>  `SyntaxError: Non-UTF-8 code starting with '\x...'`
- 问题：`SyntaxError: Non-UTF-8 code starting with '\x...'`
- 原因：代码文件不是 UTF-8 编码，或者有中文字符没有正确
- 解决办法：确保代码文件保存为 UTF-8 编码，或者删除/修改有问题的中文字符。
