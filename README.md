# NKU_thesis_graduate
南开大学硕博毕业论文模板（2024）- NKU thesis template for graduate students

## 链接
Github: [NKU_thesis_graduate](https://github.com/qianchd/NKU_thesis_graduate)

Overleaf: [NKU_thesis_graduate](https://www.overleaf.com/read/rytpskmrrhjc#f350c6)

## 历史来源
该毕业模板在互联网上有非常多版本，其最早的来源应是数学院[孙文昌老师](https://my.nankai.edu.cn/sms/swc/list.htm)制作的， 可惜原始的数院[个人网页](http://222.30.48.141/~sunwch/)已经无法访问。孙老师是早期[xeCJK](https://ctan.org/pkg/xecjk)包的作者，也基本是南开数学院学生LaTeX语言的启蒙人，大部分数学院本科生的LaTeX大概是孙老师的暑期小学期课程教授的。

本仓库主要修改自南开大学图书馆发布的[2023年版本模板](https://libpaper.nankai.edu.cn/newlist.action?encid=58)，其来源也是陈所的学长提供。初始的第一个commit即为该版本。

## 本版本新特性

现在的版本主要修改了如下几点：

- 添加2024年最新版南开大学研究生学位论文写作规范。
- 添加相应需要的字体。
- 修改授权书和原创性声明为2024年新版 (未通过相关老师校对以及验证。作者只保证目前肉眼所见和word版本基本排版一致。作者不保证按此版本提交可以通过图书馆检查)。
- 修改XeLaTeX编译下关于 Time News Roman 英文字体支持的bug。这是一个存在许多年的bug。
- 在Texlive2022、Texlive2023、MikTex等发行版下，在Windows11系统，wsl2-ubuntu 以及 Ubuntu系统下测试编译通过。

## 字体支持

若因字体缺失导致编译错误，首先解压fonts文件夹下压缩文件。

Windows下如缺字体，将fonts目录中的字体拷贝到```C:/Windows/Fonts```中。

Ubuntu中，参考以下。
```
mkdir /usr/share/fonts/thesis/
cd fonts
cp *.ttc /usr/share/fonts/thesis/
cp *.ttf /usr/share/fonts/thesis/
sudo fc-cache -fv
```

## 待办
- 因Overleaf不支持商业化字体，目前仍未适配Overleaf上XeLaTeX编译
