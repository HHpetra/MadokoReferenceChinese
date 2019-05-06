# madoko--一个轻便的Markdown在线编辑器
Madoko 是一个轻快的[Markdown]在线编辑器，使用[Koka]语言编写。这是作为新的强类型的Kako语言的一个示范程序，它的名字来源于"**Ma**/rk/**do**/wn/ in **Ko**/ka"。

Madoko可以在线使用[Madoko.net]，通过[onedrive]、[dropbox]或者[github]存储。也可以使用命令行程序在本地运行，本地运行的好处是可以指定文件储存位置，但是需要安装大量的依赖环境，包括nodejs和TexLive。
## 使用 Madoko
最佳的体验就是在线使用：<https://www.madoko.net>
或者可以用命令行运行：
* 确保你安装有[Node.js]
* 打开命令行窗口运行npm安装Madoko：  
  `npm install madoko -g`
* 安装完成后，使用以下命令简单的转换Markdown格式文件：  
  `madoko -v mydoc.mdk`
* 默认转换为`mydoc.html`。也可以转换为pdf文件，使用`-v`参数中更详细的设置：  
  `madoko --pdf -vv --odir=out mydoc`
  `--odir`参数中的`out`填写你要输出文件的路径。为了可以生成pdf文件，你需要确保已经安装有LaTex，这也是生成数学公式和目录所必须的。我们推荐安装[TexLive]发行版，包含windows、Linux和MacOSX版本。[Madoko.net]使用的同样也是这个发行版。

[TexLive]:    https://www.tug.org/texlive
[MacTeX]:     http://tug.org/mactex/
[Madoko.net]: https://www.madoko.net

## Madoko哲学

Madoko主要的设计目标是为了轻便的创作高质量网页和印刷品格式的学术文献和工业文档。同时保持约翰·格鲁伯(John Gruber)的简化和注重纯文本可读性的Markdown哲学。

Markdown的流行并不意外，它非常适合创作短文：Markdown非常简单而直接制造好看的HTML页面。但是对于其他领域更高级的使用，Markdown有些力不从心。Madoko为编辑大型文档提供了许多必要的补充。

Madoko不仅可以输出HTML页面，还可以借助LaTex输出高质量的PDF文件。尽管许多的Markdown编辑器支持这一点，但是在Madoko中已经做了许多工作来使得LaTex的生成更完善并且可以定制化。这使得用Madoko编写高质量的文章成为可能，并且可以同时生成高质量PDF和好看的HTML页面。

跟多详细内容请看[Madoko手册](http://research.microsoft.com/en-us/um/people/daan/madoko/doc/reference.html)

Have fun,
-- Daan

## 翻译

大家好，我是韦钧培（鱼人宝宝爱吃鱼）。经过苦苦的搜寻和尝试，我终于在一众Markdown编辑器中相中了Madoko这款编辑器，它完美的符合了我的需求：
* 支持简单的Markdown
* 方便输入数学公式
* 支持交叉引用，如文献引用、脚注等
既可以用来创作日常小短文，也能写帮助文档，最重要的是可以写学术文献！文本格式使得它能支持git进行版本控制。这点word做不到，word成了我的备用方案。
这么趁手的工具居然没多少人使用有点可惜。可能是没有一个完整的中文手册导致的，那么我将边学习使用，边翻译该文档。想参与的话可以提交PR，发现翻译有误的或者解释不清的地方欢迎指出。本人翻译经验不足，请多多包涵:)

[Koka]:     http://koka.codeplex.com
[dropbox]:  http://dropbox.com
[github]:   http://github.com
[markdown]: http://daringfireball.net/projects/markdown/
[onedrive]: https://skydrive.live.com/
[Node.js]: http://nodejs.org