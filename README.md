## 合肥工业大学研究生毕业设计（论文）模板
首先声明下，本项目建立在[Netcan](https://github.com/netcan/HFUT_Thesis)开发的合肥工业大学本科毕业设计模板基础上，将之进行了扩展到合肥工业大学研究生毕业设计上，在使用之前你需要安装可以编译tex的软件，Latex、visiual studio或者Anything你想用的，Linux或者Mac用户可以make做编译。

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

# 注意事项

编码方式默认为UTF-8。

这个模板是初版，大家觉得哪里不合适，可以进行contribute，也可以私信我提出意见，后期有更新的话，注意关注下，感谢支持，希望大家都能顺利毕业！