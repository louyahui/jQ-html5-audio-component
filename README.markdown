这是一个基于HTML5 和 Css3的小型web音频播放器

## 样式

此项目的第一首歌，献给光叔，致远行。

![demo-pic](http://numerhero.github.io/assets/download/jQ-html5-audio-component/demo-pic.png)

## get start

```
<link rel="stylesheet" href="xx/xx/musicMedia.min.css">

<script src="musicMedia.min.js"></script>
```

## 修改路径

默认的背景图片 和 小图片需要在js 和 sass中进行修改

```scss
$icon : "./img/icon.png";  // 默认图标
$disc : "./img/disc.png";  // 默认碟片图片
```

```javascript
defaultBg : "./img/dft-muisc-alumn-bg.jpg" // 默认背景图片
```

## 使用

```html
<section class="musicMedia-wrap just-select-text"></section>
```

在页面合适的位置 加入以上代码

并添加音乐源地址和音乐参数，以及博客一些信息

```javascirpt
$(".musicMedia-wrap").musicMedia({
        domainName : "Owen 博客", //你的博客名
        autoplay : false,    // 是否自动播放
        autoHidden : true,   // 是否自动隐藏
        defaultBg : "./img/dft-muisc-alumn-bg.jpg"             //修改默认背景路径
    },[{
      favoriteName: "Owen喜欢听的歌",
      musicList : [
        {
            title: "蓝莲花",
            singer: "许巍",
            AlbumName: "时光.漫步",
            AlbumBg: "xxxx.jpg",
            url: "xxxx.mp3"
        }
    ]},{
      favoriteName: "小城往事",
      musicList: [{
            title: "爱情转移",
            singer: "陈奕迅",
            AlbumName: "The 1st Eleven Years 然后呢？",
            url: "xxxx.mp3"
        },{
            title: "陪你度过漫长岁月",
            singer: "陈奕迅",
            AlbumName: "陪你度过漫长岁月",
            url: "xxxx.mp3"
        }]  
    }]);
```

## 新增错误处理

![pic](http://numerhero.github.io/assets/download/jQ-html5-audio-component/error.png)

如图，如果蓝莲花无法加载则会自动加载下一首或上一首 并提醒用户无法播放和禁止用户再点击播放

## 依赖

依赖于 jquery-2.2.3 版本

## 协议

MIT