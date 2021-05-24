# 合肥工业大学学位论文LaTeX模板 迁移至 [HFUTTUG/HFUT_Thesis](https://github.com/HFUTTUG/HFUT_Thesis)

## 合肥工业大学研究生毕业设计（论文）模板
首先声明下，本项目建立在[Netcan](https://github.com/netcan/HFUT_Thesis)开发的合肥工业大学本科毕业设计模板基础上，将之进行了扩展到合肥工业大学研究生毕业设计上，在使用之前你需要安装可以编译tex的软件，Windows用户可以安装Texlive 、Miktex、visiual studio，Mac用户推荐Texshop，Ctex套装不建议使用😂

# 使用方法

修改`macro.tex`文件，编辑如下内容：

```latex
% 模板设置
\newcommand{\privacy}[1][公开]{#1} % 密级
\newcommand{\type}[1][【设计或者论文】]{#1} % 类型，选填
\newcommand{\titleCna}[1][XXX]{#1} % 中文题目，默认最长12字符，查过部分换行到\titleCnb，我感觉大部分同学的题目长度都是超过12个字符，所以这部分我分为a，b两部分
\newcommand{\titleCnb}[1][XXX]{#1} % 中文题目，默认最长12字符，补充到a
\newcommand{\titleEn}[1][XXX]{#1} % 英文题目

\newcommand{\keywordsCn}[1][]{#1} % 中文关键字
\newcommand{\keywordsEn}[1][]{#1} % 英文关键字

\newcommand{\supervisor}[1][XXX\hspace{2em}教授]{#1} % 导师姓名
\newcommand{\studentID}[1][XXX]{#1} % 学号
\newcommand{\studentNameCn}[1][XXX]{#1} % 填写中文姓名
\newcommand{\studentNameEn}[1][XXX]{#1} % 填写英文姓名

\newcommand{\finishedYear}[1][\the\year]{#1} % 论文完成日期: 年
\newcommand{\finishedMonth}[1][\the\month]{#1} % 论文完成日期: 月
\newcommand{\finishedDay}[1][\the\day]{#1} % 论文完成日期: 日


\newcommand{\department}[1][计算机与信息学院]{#1} % 系名称
\newcommand{\major}[1][信号与信息处理]{#1} % 专业名称
\newcommand{\enrolmentYear}[1][【2017级】]{#1} % 入学年份
\newcommand{\object}[1][XXX]{#1} %研究方向
```

然后把自己的论文在main.tex文件下，main.tex文件已经做了很详细的注释。

可以自行编译，Linux或者Mac用户可以make做编译，Windows用户可以双击build.bat进行编译生成Pdf。

# 已知问题反馈

- `LaTeX Error: Unknown option `heading=true’ for package `ctex’`报错，由于当前所使用的 LaTeX 编译系统版本过旧或其宏包库没有更新，请或是更新 LaTeX 宏包库或是安装最新 LaTeX 编译器。如果你用的编译器是Ctex套装可能会引起这个问题，CTEX 套装已停止维护，建议安装下Texlive、Miktex或是Texshop，heading=true是ctex包下可以将章节标题设置为中文风格，这个在兼容性上不好解决，建议更换编译器。
- `Package minted error: you must have pygmentize' installed to use this packag`，这个问题可能出现在你的Python没有安装pygmentize，如果安装了pygmentize，就是你环境没有配置正确，在LaTeXTools configuration file中可以将`"texpath":"$PATH:/usr/texbin:/usr/local/bin:/opt/local/bin"`路径中加入你的pygmentize路径，即`"texpath":"$PATH:/usr/texbin:/usr/local/bin:/opt/local/bin:/Library/Frameworks/Python.framework/Versions/3.4/bin" `这里的地址视你的电脑下的地址，此处仅仅是给出示例。温馨提示：如果你的论文中不需要插入代码，此时就可以忽略这个错误，将与minted相关的包和代码全部删除即可。

# 更新说明

- `2020-04-06`  致谢部分提前，代码高亮
- `2020-04-07`  添加攻读硕士学位期间的学术活动及成果情况页面
- `2020-04-08`  对英文封面的语法进行调整

# 注意事项

- 编码方式默认为UTF-8。

- 这个模板是初版，大家觉得哪里不合适，可以进行contribute，也可以私信我提出意见，后期有更新的话，注意关注下，感谢支持，希望大家都能顺利毕业！
