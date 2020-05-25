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
