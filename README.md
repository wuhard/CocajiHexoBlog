# CocajiHexoBlog

1. npm install 
2. npm install https://github.com/CodeFalling/hexo-asset-image --save 解决图片路径找不到
3. 进入你项目根目录的node_modules\hexo-toc\lib\filter.js 中，把 28 行～31 行修改为：
     $title.attr('id', id);
    // $title.children('a').remove();
    // $title.html( '<span id="' + id + '">' + $title.html() + '</span>' );
    // $title.removeAttr('id');
    解决文章标题不跳转
4. hexo clean --> hexo s 启动服务器 --> localhost:4000

构建
hexo clean-->hexo g --> 生成的文件在public下--->上传到git或者服务器

博客编写 eg: 写一个cocoji文章
Hexo new cocaji--> 生成\CocajiHexoBlog\source\_posts\cocaji.md

下载个编辑markdown格式的编辑器 https://www.typora.io/

博客内容说明：
ctrl + / 切换编辑模式

文件头说明
---
title: Talking about the game(2)  (标题）
date: 2020-05-11 21:14:53   （日期）
tags:  game      （tag标签）
toc: true      (小标题跳转）
thumbnail: /gallery/thumbnail/aboutGame2.jpg （文章开头图片展示，路径是CocajiHexoBlog\themes\icarus-2.8.1\source\gallery\thumbnail）
---


###  1 What games do you want not to play or uninstall? ###表示3级标题

<!--more--> 表示后面的隐藏

<div align = center>

![](1.jpg)

</div>  插入图片，图片路径是文章同文件下的目录，这里是cocaji目录





